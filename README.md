# New Computer Setup

My setup for a fresh macOS Sierra machine, including my go-to front-end developer tools. This will use between 8 and 9gb of disk space.

### Contents

- [macOS setup](setup--system.md) (separate doc)
	- [Dock](setup--system.md#dock)
	- [System](setup--system.md#system-preferences)
	- [Finder](setup--system.md#finder)
- [Apps](#apps)
	- [Protection](#protection)
	- [General](#general)
	- [Office](#office)
	- [Browser](#browser)
	- [Developer apps](#developer)
	- [Other essential apps](#other-essential-apps)
	- [Additional apps](#non-essential-apps)
	- [Music](#music)
	- [Delete GarageBand](#delete-garageband)
- [Command line](setup--command-line.md) (separate doc)
- [App preferences](setup--app-prefs.md) (separate doc)

## Apps
### First: protection

- [Sophos Anti-Virus "Classic"](https://community.sophos.com/products/free-antivirus-tools-for-desktops/f/sophos-anti-virus-for-mac-home-edition/80025/where-to-download-sophos-anti-virus-sav-home-edition-9-5-2-reffered-to-as-classic-now-that-there-also-is-a-cloud-edition) - anti-virus (supported legacy version which allows scanning specific directories. the new Sophos Home will only scan the entire computer)
- [ClamXav](https://www.clamxav.com) - anti-virus and anti-malware (*paid*)
- [Micro Snitch](https://www.obdev.at/products/microsnitch/index.html) - monitor camera and mic use (*paid*)
- [Tunnelblick](https://tunnelblick.net) - OpenVPN configuration manager
	- There are many well-respected VPN providers, for example [https://privateinternetaccess.com](https://privateinternetaccess.com)
- [Suspicious Package](http://www.mothersruin.com/software/SuspiciousPackage/get.html) - Quicklook inspector for installers

### General
- [1Password](https://1password.com/downloads/) - password management (*paid* service, free direct download)
- [antiRSI](https://itunes.apple.com/us/app/antirsi/id442007571?mt=12) - encourages you to take breaks to prevent repetitive stress injuries (*paid*)
	- [my preferences](#antirsi)
- [DropBox](https://www.dropbox.com/install#downloaded) - synced file management
- [f.lux](https://justgetflux.com) - screen gammut adjuster
- [GoogleDrive desktop app](https://www.google.com/drive/download/)
- [GIF Brewery](http://gifbrewery.com/) - full-featured gif creation (frame rate/frame duration, color optimization) with video->gif conversion and screen recording
- [Harvest](https://itunes.apple.com/us/app/harvest/id506189836?mt=12) - time tracking
	- [my settings](setup--app-prefs.md#harvest)
- [MonoSnap](http://monosnap.com/welcome) - screenshot, screen video (thanks for the tip, [ten1seven](https://github.com/ten1seven)!)
- [Toggl](https://support.toggl.com/toggl-on-my-desktop/) - time tracking. Gives you a nice time sheet with each entry listed separate with its start time, end time, and duration. Nice web light-weight analytics too
	- [my settings](setup--app-prefs.md#toggl)

### Office
- [Fantastical](https://flexibits.com/fantastical) - calendar that does a number of things better than Apple's Calendar: panel with month view and a list upcoming events; Reminders integration; support multiple calendar sets, and auto-switching based on location; meaningful year view; list of all invites you haven't responded to (*paid, free trial*)
- Gmail: I make a [Fluid](http://fluidapp.com/) desktop app for `https://mail.google.com`
	- Fluid is free, but pay the $5 and the app will (automatically!) badge with the unread count and you'll have the option of a menubar app
	- [Gmail icon](resources/Ncrow-Mega-Pack-1-Gmail.icns) (courtesy of ncrow - [website](http://www.iconarchive.com/show/mega-pack-1-icons-by-ncrow/Gmail-icon.html))
	- [my settings](setup--app-prefs.md#gmail)
- [Ship](https://www.realartists.com) - GitHub issues tracker/manager (*paid, free trial*)
- [Slack](https://itunes.apple.com/us/app/slack/id803453959?mt=12) - team chat
	- turn on [All Unreads](https://get.slack.help/hc/en-us/articles/226410907)
	- study up on the [keyboard shortcuts](https://get.slack.help/hc/en-us/articles/226410907)

### Browser
- Safari  
	Extensions:
	- [1password](https://agilebits.com/onepassword/extensions) - password management
	- [GitHub Dark: Script](https://github.com/StylishThemes/GitHub-Dark-Script) via Tampermonkey - gives GitHub a dark theme
- [Firefox](https://www.mozilla.org/en-US/firefox/products/)  
	Extensions:
	- [1password](https://agilebits.com/onepassword/extensions) - password management
	- [GitHub Dark: Script](https://github.com/StylishThemes/GitHub-Dark-Script) via Greasemonkey - gives GitHub a dark theme
- [Chrome](https://www.google.com/chrome/)  
	Extensions:
			
	- [1password](https://agilebits.com/onepassword/extensions) - password management
	- [AdBlock](https://chrome.google.com/webstore/detail/adblock/gighmmpiobklfepjocnamgkkbiglidom?hl=en)
	- [Adblock for Youtube](https://chrome.google.com/webstore/detail/adblock-for-youtube/cmedhionkhpnakcndndgjdbohmhepckk?hl=en)
	- [Better History](https://chrome.google.com/webstore/detail/better-history/obciceimmggglbmelaidpjlmodcebijb?hl=en) - history with deep search; browse history by date
	- [BrowserStack](https://chrome.google.com/webstore/detail/browserstack/nkihdmlheodkdfojglpcjjmioefjahjb?hl=en) - cross-browser testing
	- [CSS Gradient Inspector](https://chrome.google.com/webstore/detail/css-gradient-inspector/blklpjonlhpakchaahdnkcjkfmccmdik?hl=en) - extends the Chrome inspector
	- [Full Page Screen Capture](https://chrome.google.com/webstore/detail/full-page-screen-capture/fdpohaocaechififmbbbbbknoalclacl?hl=en) - export screenshots of an entire webpage, no matter how long it is
	- [GitHub Dark: Script](https://github.com/StylishThemes/GitHub-Dark-Script) via Tampermonkey - gives GitHub a dark theme
	- [GitHub Plus](https://chrome.google.com/webstore/detail/github-plus/anlikcnbgdeidpacdbdljnabclhahhmd?hl=en) - adds missing functionality: repo size, file sizes, direct download links for every file, button to copy file contents
	- [Harvest](https://chrome.google.com/webstore/detail/harvest-time-tracker/fbpiglieekigmkeebmeohkelfpjjlaia?hl=en) - time tracking
	- [Quick Source Viewer](https://chrome.google.com/webstore/detail/quick-source-viewer/cfmcghennfbpmhemnnfjhkdmnbidpanb?hl=en) - a more full-featured alternative to Chrome's `View > Developer > View Source`
	- [Quick Tabs](https://chrome.google.com/webstore/detail/quick-tabs/jnjfeinjfmenlddahdjdmgpbokiacbbb?hl=en) - search open tabs' title and urls
	- [Slinky Elegant](https://chrome.google.com/webstore/detail/slinky-elegant/bmanlajnpdncmhfkiccmbgeocgbncfln) - 
	- [Spaces](https://chrome.google.com/webstore/detail/spaces/cenkmofngpohdnkbjdpilgpmbiiljjim?hl=en) - name multitab windows, and quickly switch between them based on the name
	- [WAVE Evaluation Tool](https://chrome.google.com/webstore/detail/wave-evaluation-tool/jbbplnpkjmmeebjpijfedlgcdilocofh?hl=en) - accessibility eval

### Developer apps
- [Atom](https://atom.io) - text editor (I find Sublime Text is much faster and more don't-leave-the-home-row friendly, but Atom's popular enough that it's probably worth being familiar with)
	- [settings' syncing instructions](https://pawelgrzybek.com/sync-atom-between-multiple-devices/)
- [BBEdit](http://www.barebones.com/bbedit) (*paid, free trial*) or [TextWrangler](http://www.barebones.com/products/TextWrangler/) (*free*) - text editor with great search-and-replace and great multi-file search
	- see also the [BareBones GREP cheatsheet](http://www.anybrowser.org/bbedit/grep.html)
- [GitHub Desktop](https://desktop.github.com) - I never actually use this, prefering SourceTree (linked below). On my home computer SourceTree periodically loses `push` permissions and the only fix is to open and close GitHub Desktop, so I keep it around. I think it also set me up with ssh keys on initial launch?
- [MacDown](http://macdown.uranusjr.com) - markdown editor
- [MAMP Pro](https://www.mamp.info/en/mamp-pro/) - servers (*paid, free trial*)
- [SequelPro](http://www.sequelpro.com/)
	- The icon has a messy background that looks pretty bad in the application switcher. [Here's a fix](resources/sequel pro icon fix.icns)
- Image optimizing tools:  
	- [ImageAlpha](https://pngmini.com) - optimize pngs that have transparency
	- [ImageOptim](https://imageoptim.com/mac) - optimize imagesons folder):
- **Simulator** - an iOS emulator (#facepalm@productnameteam) that comes with XCode (see below)
	- If Spotlight isn't finding it, or just for general ease of access in Finder, make an alias in the Applications folder:

			ln -s /Applications/Xcode.app/Contents/Developer/Applications/Simulator.app /Applications
- [SourceTree](https://www.sourcetreeapp.com) - git and hg client
- [Sublime Text](https://www.sublimetext.com/) - text editor
	- If you've already registered but lost your license, [get it emailed to you](https://www.sublimetext.com/retrieve_key)
	- [settings' syncing instructions](https://packagecontrol.io/docs/syncing)
	- If you're new, watch this [tutorial video](https://code.tutsplus.com/courses/perfect-workflow-in-sublime-text-2)
	- [Handy shortcuts](https://www.viget.com/articles/my-overused-sublime-text-keyboard-shortcuts)
	- My packages:
		- `AdvancedNewFile` - create new files in the same location as the current document. also delete, copy, and rename files
		- `Boxy Theme` - super configurable theme
		- `BracketHighlighter` - configurable highlighting for code block opens and closes
		- `Clickable URLS` - mouse equivalent of "Open URL"
		- `Color Highlighter` - shows color values colors in markup and stylesheets
		- `Craft-Twig` - syntax highlighting for twig documents, with Craft-specific support. I use this for all html files
		- `Emmet` - [Emmet](http://emmet.io/) (see also the [cheatsheet](http://docs.emmet.io/cheat-sheet/))
		- `HTML-CSS-JS Prettify` - beautifier running js-beautify
		- `Origami` - flexible window tiling
		- `Pretty JSON` - JSON beautifier
		- `Status Bar File Size` - shows the file size in the status bar
		- `SublimeLinter`
		- `A File Icon` - sidebar filetype-based 
		- `WakaTime` - automatic time tracking
	- I use the pre-installed "Monokai" theme, because it has the best [LESS]() support I've seen
	- And I turn on scrolling past the end of documents: open `Preferences.sublime-settings -- User` with `command ,` and add `"scroll_past_end":true`
- [Virtual Box](https://www.virtualbox.org/wiki/VirtualBox)
	- [Windows IE/Edge VMs](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)
- [XCode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
	- [my settings](setup--app-prefs.md#xcode)
- [XScope](http://xscopeapp.com) - tools for measuring and inspecting stuff on the screen

### Additional apps
- **Afloat**, via SIMBL - make windows float on top, and control their transparency
	- [Installation instructions](http://www.perfectlyrandom.org/2016/10/23/always-on-top-in-macos-sierra/)
	- I mostly use this for keeping an eye on command line activity, but it's also useful for comparing a site to a comp
- [AppTrap](http://onnati.net/apptrap/) - extension for automatically deleting associated files when an app is deleted
- [Auto Mute](http://auto-mute.com/download/) - mutes system on logout and shutdown, to prevent startup chime
- [BarTender](https://www.macbartender.com/) - hide menubar apps (*paid, free trial*)
	- [my menubar, after installing everything in this doc](#bartender)
- [BetterTouchTool](https://www.boastr.net/) - has all sorts of powers, notably for resizing and moving windows when the cursor is over the window (don't have to grab the title bar to move, don't have to grab the edge to resize; *paid*)
	- [my settings](setup--app-prefs.md#bettertouchtool)
- [CoconutBattery](http://www.coconut-flavour.com/coconutbattery/) - menubar battery meter
	- [my settings](setup--app-prefs.md#coconutbattery) - I show the time, state, and percentage
- [ControlPlane](https://www.controlplaneapp.com/) - context-dependent actions
	- [my settings](setup--app-prefs.md#controlplane) - I use this to save time by automatically opening my go-to work apps when I get to the office, but more importantly I use it to automatically connect to my VPN when on the public networks I frequent (e.g. my town wifi, the library, etc)
- [Day-O](http://www.shauninman.com/pendium/) - menubar clock replacement with dropdown calendar (skip if using Fantastical)
- [EasyFind](http://www.devontechnologies.com/products/freeware.html) - powerful search tool
- [InsomniaX](http://semaja2.net/projects/insomniaxinfo/) - disable sleep, including lid sleep
- [Isolator](https://www.willmore.eu/software/isolator/) - basic menubar-based screen shader
	- [my settings](setup--app-prefs.md#isolator)
- [Little Snitch](https://www.obdev.at/products/littlesnitch/index.html) - monitor network connections (*paid, free time-limited version*)
- [mySIMBL](https://github.com/w0lfschild/mySIMBL) - manager for SIMBL plugins (plugins to customize and tweak macOS)
	- [my plugins](#mysimbl) - I use Afloat, cDock, colorfulSidebar, and NotificationClear
- [Noizio](http://noiz.io/) - ambient sounds with custom, shareable mixes
	- here's [the starting point](resources/Hillsborough Rd.nzm) I made for messing around with while I work
- [qlmarkdown](https://github.com/toland/qlmarkdown) - Quicklook plugin to display Markdown
- [SlimBatteryMonitor](http://www.orange-carb.org/SBM/index.html) - menubar battery meter
	- [my settings](setup--app-prefs.md#slimbatterymonitor) - I just show the image
- [Spectacle](https://www.spectacleapp.com/) - window resizing
	- [my settings](setup--app-prefs.md#spectacle)
- [Trailer](https://ptsochantaris.github.io/trailer/) - GitHub issue monitor for Mac (menubar), iOS, watchOS
- [TinkerTool](https://www.bresink.com/osx/TinkerTool.html) - access to hidden system preferences
	- [my settings](setup--app-prefs.md#tinkertool)
- [TotalSpaces](https://totalspaces.binaryage.com/) - grid spaces (*paid*)
- [Vienna](https://github.com/ViennaRSS/vienna-rss) - free, open source RSS/Atom reader (useful for testing feeds during development)
- [WiFi Signal](https://itunes.apple.com/us/app/wifi-signal/id525912054?mt=12) - menubar signal meter
	- [my settings](setup--app-prefs.md#wifi-signal) - I just show the strength as a number
	
### Non-essential apps
- [Air Display](https://avatron.com/applications/air-display/) - use up to 4 other Macs and/or iOS devices as external monitors over WiFi or USB (*paid, free trial*)
- [Rocket](http://matthewpalmer.net/rocket/) - System-wide Slack-like emoji… `:open-mouth:` ➡️ 😮

### Music
- [LastFM scrobbler](http://www.last.fm/about/trackmymusic#desktop)
- [Sonos Controller](http://www.sonos.com/en-us/controller-app) for Sonos speakers
	- and [airsonos](https://github.com/stephen/airsonos) utility for using Sonos speakers as Airplay speakers (i.e. for streaming a Mac's system sound, or streaming sound from an iOS app)
		- as of this writing, requires the easy fix from [airsonos#316 (comment)](https://github.com/stephen/airsonos/issues/316#issuecomment-255663049) or, if that doesn't work, the more involved one from [airsonos#342 (comment)](https://github.com/stephen/airsonos/issues/342#issuecomment-295770479)
- [Spotify](https://www.spotify.com/us/download/other/)

### Delete GarageBand

Trash these (these are the GarageBand files on a clean Sierra install. Verify the file list with [CleanApp](http://www.syniumsoftware.com/cleanapp) or use EasyFind to search for GarageBand.)

```/Applications/GarageBand

/Library/Application Support/GarageBand

/Library/Audio/Apple Loops/Apple/Apple Loops for GarageBand

/Library/Receipts/com.apple.pkg.GarageBand_AppStore.bom

/Library/Receipts/com.apple.pkg.GarageBand_AppStore.plist

/System/Library/Receipts/com.apple.pkg.MAContent10_AssetPack_0325_AppleLoopsGarageBand1.bom

/System/Library/Receipts/com.apple.pkg.MAContent10_AssetPack_0325_AppleLoopsGarageBand1.plist

~/Library/Application Scripts/com.apple.STMExtension.GarageBand

~/library/containers/com.apple.STMExtension.GarageBand
```

---

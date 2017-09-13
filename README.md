# New Computer Setup

My setup for a fresh macOS Sierra machine, including my go-to front-end developer tools. This will use something under 10gb of disk space.

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

- [Sophos Anti-Virus "Classic"](https://community.sophos.com/products/free-antivirus-tools-for-desktops/f/sophos-anti-virus-for-mac-home-edition/80025/where-to-download-sophos-anti-virus-sav-home-edition-9-5-2-reffered-to-as-classic-now-that-there-also-is-a-cloud-edition) - anti-virus (supported legacy version which allows scanning specific directories - the newer Sophos Home will only scan the entire computer)
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
- [Mackup](https://github.com/lra/mackup) - backup your app settings, and sync them across multiple computers
- [MonoSnap](http://monosnap.com/welcome) - take and leave notes on screenshots
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

### Browsers
- Safari
- [Safari Technology Preview](https://developer.apple.com/safari/technology-preview/)
- [Chrome](https://www.google.com/chrome/)
- [Chrome Canary](https://www.google.com/chrome/browser/canary.html?platform=mac)
- [Firefox](https://www.mozilla.org/en-US/firefox/products/)
- [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)

### Browser Extensions

- Cross-browser

	- [1password](https://agilebits.com/onepassword/extensions) - password management
	- [AdBlock](https://getadblock.com)

	- GitHub extensions
		- [GitHub code folding](https://github.com/Mottie/GitHub-userscripts/wiki/GitHub-code-folding) - A userscript that adds code folding to GitHub files
		- [GitHub custom navigation](https://github.com/Mottie/GitHub-userscripts/wiki/GitHub-custom-navigation) - A userscript that allows you to customize GitHub's main navigation bar. I link
			- Request PR reviews (`https://github.com/pulls?q=review-requested:username`)
			- Assigned issues (`https://github.com/issues/assigned`)
			- My gists (`https://gist.github.com/username`)
		- [GitHub sort content](https://github.com/Mottie/GitHub-userscripts/wiki/GitHub-sort-content) - A userscript that makes some lists & markdown tables sortable
		- [GitHub Dark: Script](https://github.com/StylishThemes/GitHub-Dark-Script) via Tampermonkey - gives GitHub a dark theme
			- I use the color `#7AAACF`
		- [GitHub reveal header](https://github.com/Mottie/GitHub-userscripts/wiki/GitHub-reveal-header) - A userscript that reveals the header when hovering near the top of the screen
		- [GitHub search autocomplete](https://github.com/Mottie/GitHub-userscripts/wiki/GitHub-search-autocomplete) - A userscript that adds autocomplete search filters to GitHub

	
- Chrome-specific

	- [Adblock for Youtube](https://chrome.google.com/webstore/detail/adblock-for-youtube/cmedhionkhpnakcndndgjdbohmhepckk?hl=en)
	- [Better History](https://chrome.google.com/webstore/detail/better-history/obciceimmggglbmelaidpjlmodcebijb?hl=en) - history with deep search; browse history by date
	- [BrowserStack](https://chrome.google.com/webstore/detail/browserstack/nkihdmlheodkdfojglpcjjmioefjahjb?hl=en) - cross-browser testing
	- [CSS Gradient Inspector](https://chrome.google.com/webstore/detail/css-gradient-inspector/blklpjonlhpakchaahdnkcjkfmccmdik?hl=en) - extends the Chrome inspector
	- [Full Page Screen Capture](https://chrome.google.com/webstore/detail/full-page-screen-capture/fdpohaocaechififmbbbbbknoalclacl?hl=en) - export screenshots of an entire webpage, no matter how long it is
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
	- Some packages I'd recommend to any front-end developer:
		- `A File Icon` - excellent sidebar icon
		- `AdvancedNewFile` - create new files in the same location as the current document. also delete, copy, and rename files
		- `Boxy Theme` - super configurable theme
		- `BracketHighlighter` - configurable highlighting for code block opens and closes
		- `Clickable URLS` - mouse equivalent of "Open URL"
		- `Color Highlighter` - shows color values colors in markup and stylesheets
		- `Copy Relative Path`
		- `Craft-Twig` - syntax highlighting for twig documents, with Craft-specific support. I use this for all html files
		- `CSS Unminifier`
		- `Dotfiles Syntax Highlighting`
		- `Emmet` - [Emmet](http://emmet.io/) (see also the [cheatsheet](http://docs.emmet.io/cheat-sheet/))
		- `ERB Snippets`
		- `Focus File on Sidebar` - open sidebar and focus on the current file
		- `Git Blame` - show a blame pop-up, with a button to quickly see the blame commit
		- `GitGutter` - show `+`/`-` Git diffs in the gutter
		- `GitStatusBar` - compact git info in the statusbar
		- `HTML-CSS-JS Prettify` - HTML/CSS/JavaScript prettifier running js-beautify
		- `LESS` - LESS syntax highlighting
		- `LoremIpsum` - generate lorem ipsum text
		- `Open URL` - option-double-click on a path to open it in the browser
		- `Origami` - ultraflexible window tiling
		- `Pretty JSON` - Prettiffy/Query/Goto/Validate/Lint JSON
		- `Status Bar File Size`
		- `SublimeLinter` - interactive code linting
		- `Sync View Scroll` - sync scrolling of multiple open files (plays nice with Origami!)
		- `Syntax Highlighting for PostCSS`
		- `Syntax Manager` - assigns syntax based on file extension (essential!), and lets you specify syntax-specific settings
		- `TodoReview` - review todo (and other) comments
		- `WakaTime` - automatic time tracking
	- I use the `One Dark` theme. For a long time before finding The One I use Sublime's pre-installed "Monokai" theme, because I liked its [LESS](http://lesscss.org/) coloring
	- I use the `Inconsolata-dz` [Powerline font](https://github.com/powerline/fonts)
	- And I turn on scrolling past the end of documents, turn off word wrap by default, increase default font size and line spacing, use a large solid caret, highlight the current line, and more. You can check out [my preferences file](Preferences.sublime-settings) (n.b: the "match_brackets" preferences are to allow BracketHighlighter to do the highlighting, and "theme" preferences are Boxy customization)

- [Virtual Box](https://www.virtualbox.org/wiki/VirtualBox)
	- [Windows IE/Edge VMs](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)
- [XCode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
- [XScope](http://xscopeapp.com) - tools for measuring and inspecting stuff on the screen (*paid, free trial*)

### Additional apps
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
- [mySIMBL](https://github.com/w0lfschild/mySIMBL) - manager for SIMBL plugins (plugins to customize and tweak macOS). I use (install these via mySIMBL - links just for screenshots and documentation)
	- [binventory](https://github.com/w0lfschild/binventory_SIMBL) - badge the Trash icon with the number of files in it
	- [cDock](https://github.com/w0lfschild/cDock) - customize the Dock appearance
	- [colorfulSidebar 9](https://github.com/w0lfschild/colorfulSidebar_9) - colored icons in the sidebar of Finder windows
	- [darkNC](https://github.com/w0lfschild/darkNC) - dark theme for the Notification Center
	- [NotificationClear](https://github.com/w0lfschild/NotificationClear) - adds a button to the Notification Center that clears all notifications
	- SpotlightSIMBL - add plugins to Spotlight. Requires [Flashlight](https://github.com/nate-parrott/Flashlight)
	- [Afloat](https://github.com/w0lfschild/Afloat) currently crashes my computer
- [Muzzle](https://muzzleapp.com/) - turns on Do Not Disturb when screensharingm
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

# Setting up a new computer

## macOS setup

### Dock

I take almost all of the defaults out the dock, make it smaller, and move it to the left

<img src="resources/images/dock.png" width="400px"/>

and change the double-click behavior

<img src="resources/images/dock preferences.png" width="400px"/>

and add spacers to the app side of the dock:  

	```
	defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}'; killall Dock
	```
	
(you can also add spacers to the documents side of the dock… but why?)
	
	```
	defaults write com.apple.dock persistent-others -array-add '{tile-data={}; tile-type="spacer-tile";}'; killall Dock
	```
	
and I make some Dock tweaks with TinkerTool ([see below](#tinkertool)). 	
Final result:

<img src="resources/images/dock final.png" width="50px"/>

### System

- **General** (appearance: graphite; always show the scroll bars; click to jump to that spot):

	<img src="resources/images/appearance.png" width="400px"/>

- **desktop & screen saver**:  
	- plain background

		<img src="resources/images/desktop.png" width="400px"/>
		<img src="resources/images/screensavers.png" width="400px"/>
		
	- screensaver hotcorner

		<img src="resources/images/screensaver hotcorners.png" width="400px"/>
		
	- [ported afterdark screen savers](resources/ported-afterdark-screen-savers.zip)
		- final frontier:

			<img src="resources/images/screensavers - final frontier.png" width="200px"/>
		
		- flying toasters:

			<img src="resources/images/screensavers - flying toasters.png" width="200px"/>
		
		- moire:

			<img src="resources/images/screensavers - moire 1.png" width="200px"/>
			<img src="resources/images/screensavers - moire 2.png" width="200px"/>
		
		- mowing man (*paid* - [registration link](http://en.infinisys.co.jp/download/index.shtml)):
		
			<img src="resources/images/screensavers- mowing man.png" width="200px"/>  
		
		- starry night (*paid*):

			<img src="resources/images/screensavers- starry night.png" width="200px"/>

- spotlight (turn off lookup):

	<img src="resources/images/turn off spotlight lookup.png" width="400px"/>

- notifications:

	<img src="resources/images/notifications.png" width="400px"/>
	
	And as you use the computer update the app preferences here, unchecking "Show in Notification Center" when possible so that Notifation Center doesn't fill up with unnecessary clutter.

- displays:

	<img src="resources/images/color.png" width="400px"/>

- energy saver:

	<img src="resources/images/battery.png" width="400px"/>

- keyboard:

	<img src="resources/images/keyboard.png" width="400px"/>
	<img src="resources/images/keyboard- shortcuts.png" width="400px"/>

- trackpad:

	<img src="resources/images/click.png" width="400px"/>
	<img src="resources/images/scroll.png" width="400px"/>
	<img src="resources/images/gestures.png" width="400px"/>

- date & time (assumes Day-O is installed):

	<img src="resources/images/time.png" width="400px"/>
	<img src="resources/images/clock + day-o.png" width="400px"/>

- accessibility:

	<img src="resources/images/accessibility.png" width="400px"/>

- internet accounts: add your accounts!

### Finder

- prefs:

	<img src="resources/images/finder prefs- general.png" width="200px"/>
	<img src="resources/images/finder prefs- sidebar.png" width="200px"/>
	<img src="resources/images/finder prefs- advanced.png" width="200px"/>  

- [folder icons](resources/folder-icons-for-dock.zip):  

	<img src="resources/images/dock icons.png" width="100px"/>

- view options:

	- Default:

		<img src="resources/images/finder view option defaults.png" width="200px"/>
	
	- Downloads:

		<img src="resources/images/downloads folder view options.png" width="200px"/>
	
	- Applications:

		<img src="resources/images/applications folder view options.png" width="200px"/>

- toolbar and window bars: show the path bar and status bar, and add to the toolbar apps I commonly want to drag and drop things onto

	<img src="resources/images/finder window.png" width="400px"/>
	
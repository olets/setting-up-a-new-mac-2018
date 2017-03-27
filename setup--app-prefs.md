
## App preferences

- ####antiRSI:

	A one-hour schedule 

	<img src="resources/images/antirsi preferences.png" width="400px"/>

- ####Bartender

	This is my menubar
	<img src="resources/images/bartender hidden.png" width="400px"/>
	
	And this is what's hidden by Bartender
	<img src="resources/images/bartender revealed.png" width="400px"/>
	
- ####BetterTouchTool:

	<img src="resources/images/bettertouchtool- general.png" width="400px"/>
	<img src="resources/images/bettertouchtool- window snapping.png" width="400px"/>
	<img src="resources/images/bettertouchtool- windows.png" width="400px"/>

- ####CoconutBattery:

	<img src="resources/images/coconutbattery preferences.png" width="400px"/>

- ####ControlPlane:

	set up automatic VPN on commonly used public networks (e.g. coffee shops, city wifi, etc)

	- in [Script Editor](file:///Applications/Utilities/Script Editor.app), create two new documents and save them as scripts or applications:

		- The connect script:  
		 
			```
			tell application "Tunnelblick"				connect "US East"				get state of first configuration where name = "US East"				repeat until result = "CONNECTED"					delay 1					get state of first configuration where name = "US East"				end repeat			end tell
			```
		- The disconnect script:  
		
			```
			tell application "Tunnelblick"				disconnect "US East"				get state of first configuration where name = "US East"				repeat until result = "EXITING"					delay 1					get state of first configuration where name = "US East"				end repeat			end tell
			```	
	- In ControlPlane's preferences: Under "Evidence Sources," add "Nearby WiFi Network"
	- Under "Rules," choose "Add 'Nearby WiFi Network' Rule" > "WiFi SSID," select your target network, and say OK (note: the first time you add a given network you must be connected to it). Set confidence to 100%
	- Under "Actions," add two of "Application Actions" > "Open File or Application"
		- For one, select your VPN connect script/application, the relevant Context, and "On arrival"
		- For the other, select your VPN disconnect script/application, the same Context, and "On departure"

- ####Harvest:

	<img src="resources/images/harvest preferences.png" width="400px"/>

- ####Isolator:

	<img src="resources/images/isolator- general.png" width="400px"/>
	<img src="resources/images/isolator- menu icon.png" width="400px"/>
	<img src="resources/images/isolator- background windows.png" width="400px"/>
	<img src="resources/images/isolator- updates.png" width="400px"/>
	
- ####MySIMBL:

	Install plugins by clicking "Discover"
	
	<img src="resources/images/simbl- discover.png" width="400px"/>
	
	and go to Wolf's plugins
	
	<img src="resources/images/simbl- wolf.png" width="400px"/>
	
	I add **Afloat**, **cDock**, **colorfulSidebar**, **Notification Clear**.
	
	You may need to turn off System Integrity Protection (SIP) during installation. mySIMBL should tell you how to do that. It's:
	
	- Restart the computer while holding down Command R to boot into Recovery Mode
	- Once the computer has started: From the Utilities menu select "Terminal"
	- `csrutil disable; reboot`
	- After installing SIMBL plugins, reenable SIP by booting into recovery mode and running `csrutil enable; reboot`

	1. **Afloat** lets you keep windows on top of others and adjust individual windows' transparency.

		<img src="resources/images/afloat.png" width="400px"/>
	
	1. **cDock** lets you theme the Dock. I use it to completely remove the Dock's background
	
		<kbd><img src="resources/images/cdock- prefs.png" width="400px"/></kbd>
		
		The result:
	
		<img src="resources/images/cdock- dock.png" width="80px"/>
	
	1. **colorfulSidebar** colors the sidebar icons. You can customize the icons - here it is with the defaults:
	
		<img src="resources/images/colorfulsidebar.png" width="200px"/>
		
	1. **Notification Clear** adds a "clear" button to clear all Notification Center notifications in one click.
	
		<img src="resources/images/notificationclear.png" width="200px"/>

- ####SlimBatteryMonitor:

	<img src="resources/images/slimbatterymonitor preferences.png" width="400px"/>

- ####Spectacle:

	<img src="resources/images/spectacle preferences.png" width="400px"/>

- ####TinkerTool:

	<img src="resources/images/tinkertool- 1 finder.png" width="400px"/>
	<img src="resources/images/tinkertool- 2 dock.png" width="400px"/>
	<img src="resources/images/tinkertool- 3 desktop.png" width="400px"/>
	<img src="resources/images/tinkertool- 4 safari.png" width="400px"/>

- ####Toggl:

	<img src="resources/images/toggl preferences.png" width="400px"/>

- ####Wifi Signal:

	<img src="resources/images/wifi signal preferences.png" width="400px"/>

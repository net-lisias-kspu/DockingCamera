# Docking Camera (KURS) /L Unofficial

Built-in cameras in every docking ports and standalone Camera for any place. Allows usage modes: "standard camera", "follow me", "look at current target" "look from target", "look at me" (from any point)

Unofficial fork by Lisias.


## In a Hurry

* [Latest Release](https://github.com/net-lisias-kspu/DockingCamera/releases)
	+ [Binaries](https://github.com/net-lisias-kspu/DockingCamera/tree/Archive)
* [Source](https://github.com/net-lisias-kspu/DockingCamera)
	+ [Unity Project](https://github.com/net-lisias-kspu/DockingCamera-Unity)
		- On a separated repository due licensing issues.  
* Documentation
	+ [Project's README](https://github.com/net-lisias-kspu/DockingCamera/blob/master/README.md)
	+ [Install Instructions](https://github.com/net-lisias-kspu/DockingCamera/blob/master/INSTALL.md)
	+ [Change Log](./CHANGE_LOG.md)
	+ [TODO](./TODO.md) list


## Description

Once upon a time there was LAZOR mod from famous Romfarer, which included a useful docking camera, that displays the videostream a small window in the main flight scene. However, it has not been updated for a long time, and refused to work in recent versions of the game (or I could not start it). Nevertheless, *[the original author]* liked it output style of information and *[the original author]* was bored without this service. That in turn has led me to attempt to revive the aforementioned docking camera. And YES, *[the original author]* knew about Docking Port Alignment Indicator, HullCamVDS, cameras for RasterPropMonitor etc. But *[the original author]* do not knew about any working cameras in window.

Docking Camera can be integrated to any part (MM patch enclosed for the docking port modules). It looks ahead by the vertical axis of the vessel's and displays a minimum of necessary info for the docking maneuver - namely, range, speed, angle, alignment and when the correct trajectory occurred - time prior to docking with the mark that such trajectory will lead our vessel to dock without additional actions (small lamp will become green and will show time to docking). camera window has three size presets. It also has three viewing modes: colour, Black and white and infrared. Powered zoom function. Also, there is a button to remove flight data from the screen.

Furthermore, effect of television interference can be added. The range of the camera, parameters of night vision (RSMA) and presence of noise - can be configured through CFG. Camera requires a target to operate.

In addition the ugly external camera enclosed. It can show videostream only and also has three modes of vision and is able to rotate on two axes. For cameras, installed under the belly of the aircraft (which gets inverted upside down) there is the mode of rotation of the image. In the CFG of the partcamera some meshes could be configured for use with other camera model.

All cameras have a title with its number, and also can work a few pieces at a time. Docking camera reporting its target on its window title.

There is an experiment on part camera - a try to reproduce a surveillance (spy) activity. You need to be at a distance less than 1000 m near any targetable thingie, catch it on camera's screen and targeted. press "⦿" button. A ray will be shoot. If all requirements have met and there are no obstacle on ray's path - you'll should get experiment results, if something wrong - you just spend one bullet.  Experiments is limited by bullets (4 yellow balls around cam, disappearing one by one each time). I thought it will be interesting if contracts.

Camera has 3 presets of shaders (noisy TV 1960th style, TV 1980th style  and standard (color, b/w and nightvision). available via button, appearing when blizzy toolbar is installed. 

Also, by toolbar button you could find info about nearby cameras installed on other vessels in transmission range. If camera has been activated on some vessel, but you drive other one - a new window from distant camera will appear when distance from first one will become less than 2500 (or 10k (customisable)). 

If you want you can use "look at me" mode by activating it on distant camera. "Targetcam"  and "follow me" modes on your active vessel (set camera position using scrollers).

The cameras can transmit the videostream to nearby vessels, but only at a distance of up to 2 500 meters. You can change this unload range via toolbar button.


## Installation

Detailed installation instructions are now on its own file (see the [In a Hurry](#in-a-hurry) section) and on the distribution file.

## License:

Until 1.2.1.1 for KSP 1.2: CC-BY-SA 4.0I, [source](https://github.com/net-lisias-kspu/DockingCamera/tree/Source/CC-BY-SA).

From 1.3.3.1 for KSP 1.3.1 and newer, CC-BY-NC-SA 4.0I.

Please note the copyrights and trademarks in [NOTICE](./NOTICE).


## UPSTREAM

* [DennyTX](https://forum.kerbalspaceprogram.com/index.php?/profile/92389-dennytx/) ROOT
	+ [Forum](https://forum.kerbalspaceprogram.com/index.php?/topic/124475-*/) 
	+ [SpaceDock](https://spacedock.info/mod/1542)
	+ [Github](https://github.com/DennyTX/DockingCam)
* [linuxgurugamer](https://forum.kerbalspaceprogram.com/index.php?/profile/129964-linuxgurugamer/) Current Maintainer
	+ Forum
		- [First](https://forum.kerbalspaceprogram.com/index.php?/topic/166305-*/)
		- [Second](https://forum.kerbalspaceprogram.com/index.php?/topic/184038-*/)
	+ [SpaceDock](https://spacedock.info/mod/?????/?????)
	+ [Github](https://github.com/????/????/)

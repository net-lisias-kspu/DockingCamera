# Docking Camera (KURS) :: Change Log

* 2020-0908: 1.3.7.5 (linuxgurugamer) for KSP 1.10.1
	+ Added settings to enable/disable the cross, summary data, detail text data and rotators
	+ Added setting for default window size
	+ Thanks to Twitch user @HansAcker for some Vector3D code to help show the proper distances from the x,y,z
	+ Removed static from camera without a target.
	+ Added toggles to window for the main options listed above
	+ Added velocity indicator
* 2020-0904: 1.3.7.4 (linuxgurugamer) for KSP 1.10.1
	+ Removed unused assets folder
* 2020-0803: 1.3.7.3 (linuxgurugamer) for KSP 1.10.1
	+ Fixed camera by replacing "Camera 01" with "UIMainCamera"
* 2019-1202: 1.3.7.2 (linuxgurugamer) for KSP 1.8.1
	+ Converted two textures from DXT3 to DXT5
* 2019-1201: 1.3.7.1 (linuxgurugamer) for KSP 1.8.1
	+ Fixed nullref when going into flight scene
	+ Fixed "Zoom:" position in slideout window
* 2019-1201: 1.3.7 (linuxgurugamer) for KSP 1.8.1
	+ Updated for KSP 1.8
* 2019-0905: 1.3.6.3 (linuxgurugamer) for KSP 1.7.3
	+ Fixed range settings in settings page, to only show one of the two ranges to be active
	+ Fixed long range setting causing vessel coming into range having it's speed matched to that of the active vessel
* 2019-0824: 1.3.6.2 (linuxgurugamer) for KSP 1.7.3
	+ Added support for the ClickThroughFix
* 2019-0804: 1.3.6.1 (linuxgurugamer) for KSP 1.7.3
	+ Fixed bug where if the second sliding window was open when the camera was closed, opening the camera again would sometimes (depending on the shader) show shadow buttons
	+ Thanks to forum user @sirkut for this:
		- Made the docking camera configurable as a general purpose camera.
	+ Added a dev mode for modders and players to be able to determine the correct values for the camera position
		- (see the ReadMe for complete instructions)
	+ Added two models to choose from for displaying the camera location, a camera and a node.  The model is selected in the stock game settings page, and only takes effect on windows when they are opened.
	+ Fixed issue with two or more cameras on the same part
	+ Added: transformModification for a special case where the transform for the camera needs to not be changed
	+ Cross stock in sliding window is overridden by settign???
	+ Renamed shaders to consistant naming: DockingCamera/(name)
	+ Added InstallChecker
	+ Changed display of shader to remove the first part of the name (before the slash)
* 2019-0614: 1.3.6 (linuxgurugamer) for KSP 1.7.1 PRE-RELEASE
* 2019-0531: 1.3.5 (linuxgurugamer) for KSP 1.7.1
	+ Removed log spam
	+ Add check for vessels undocking
	+ Fixed check for vessels with cameras nearby
	+ Changed default Noise setting to false for docking cameras
	+ Added option to use the standard KSP skin
	+ Removed Blizzy option from settings page (now controlled by ToolbarController)
	+ Added UI scaling
	+ Replaced the lower-right button which cycled through the sizes with two new buttons, one to increase and one to decrease the size
	+ Added an "x" to close button in upper right
	+ Fixed the rotators so they won't overlap in larger windows
	+ Changed the KURS Camera Info window to only show data
	+ Updated the wording in the window to properly reflect 1 or multiple (putting an s after vessel when appropriate)
	+ Added InitWindow() to docking camera Activate()
* 2019-0426: 1.3.4.1 (linuxgurugamer) for KSP 1.7.0
	+ Updated for 1.7.0
* 2019-0426: 1.3.4 (linuxgurugamer) for KSP 1.7.0
	+ Nightvision and TV shaders are working again
	+ TV shader replaced by a CRT shader
	+ Updated obsolete code to new standards
	+ Removed old Noise shaders, were replaced by code long time ago
	+ Changed functionality of aux window when resizing, it now stays the way it is (ie: if open, will reopen when resizing is complete)
	+ Added additional larger size
	+ Changed camera rotation from 180 to 90 degrees (for the camera part)
	+ Removed extra level of directory from release (removed the OLDD directory)
	+ Renamed directory to DockingCamKURS
	+ Rewrote the ReadMe.md
* 2018-0709: 1.3.3.2 (linuxgurugamer) for KSP 1.3.1
	+ This release adds back the missing PNG files to make the mod work.
	+ the nightvision and TV shaders are NOT functional at this time
* 2018-0215: 1.3.3.1 (DennyTX) for KSP 1.3.1
	+ REBORN.
		- Recompiled for KSP 1.3.1
		- Fixed problem with texture creational while -force-d3d11 (DX11) (post with problem)
		- assets will load only once
		- reduced spam to log
		- DELETE previous versions by me or linuxgurugamer before installation
	+ If installing by CKAN, no need to manually delete old versions
* 2017-1022: 1.3.2 (linuxgurugamer) for KSP 1.3.1
	+ Added ability to rotate the docking camera
	+ Added zoom to docking camera
* 2017-1020: 1.3.1.3 (linuxgurugamer) for KSP 1.3.1
	+ Fixed nullref when instantiating vessel
* 2017-1009: 1.3.1.2 (linuxgurugamer) for KSP 1.3.1
	+ No changelog provided
* 2017-1009: 1.3.1.1 (linuxgurugamer) for KSP 1.3.1
	+ No changelog provided
* 2018-0513: 1.1.6.6 (linuxgurugamer) for KSP 1.3.1
	+ Recompile by LGG for 1.4

# Docking Camera (KURS) :: Change Log

* 2021-0721: 1.3.8.2 (linuxgurugamer) for KSP 1.12.1
	+ Fixed OnboardCamera to work in orbit
	+ Added Assemblyfileversion
	+ Updated project info
* 2021-0311: 1.3.8.1 (linuxgurugamer) for KSP 1.11.1
	+ Closes # 23
	+ Added ModuleCargoPart for KSP 1.11
* 2020-1208: 1.3.8 (linuxgurugamer) for KSP 1.10.1
	+ Increase size of info window
	+ Merged in changes from forum user @Dehim (github @Dehim1) with alternate mode
	+ Added help window for alt mode
	+ Added setting for alt mode
	+ Added toggle for alt mode on info window
	+ Rewrote config save, now saves to a .cfg in PluginData
	+ Now remembers last size of camera window
	+ Now remembers last location of camera window
* 2020-1121: 1.3.7.9 (linuxgurugamer) for KSP 1.10.1
	+ Reverted cullingmask change
* 2020-1116: 1.3.7.8 (linuxgurugamer) for KSP 1.10.1
	+ Adjusted the cullingmask for the markercam
* 2020-1115: 1.3.7.7 (linuxgurugamer) for KSP 1.10.1
	+ Fixed typo of asset name for targetpoint
	+ Thank to github user @wile1411 for all of the following:
		- Reordered PartCamera.cs Activate() function. It was also missing the InitTextures() which was causing the Target marker to not load.
		- Added ActionGroup for camera activation to both part modules
		- Corrected the shader reference path to: 'Legacy Shaders/Particles/Additive '. Was causing NRE errors if bullets or Target ray buttons were used.
		- Added user config option to set EC amount for camera usage. Was hard coded to 0.02. Updated part cfg files to match.
		- Found a logic hole in the PartCameraModule. When a camera isEnabled (after being activated()) it does regular checks for electric charge. Once EC gets to zero, the mod will deactivate the camera (docking cameras are unaffected) and set isEnabled & _isPowered to "FALSE".
		- In this state, there is no way to get back to IsEnabled = true due to there being a power state check before allowing a user to enable a camera. No EC checks are ever run again and the camera cannot be used.
		- Added code to do an ECcheck before trying to enable the camera to avoid this issue.
		- Fixed the kerbals being seen through parts by fixing the cullingMaskLayer
* 2020-1013: 1.3.7.6 (linuxgurugamer) for KSP 1.10.1
	+ Converted textures to dds
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
* 2018-0513: 1.1.6.6 (linuxgurugamer) for KSP 1.4
	+ Recompile by LGG for 1.4
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
* 2016-11-18: 1.2.1.1 (DennyTX) for KSP 1.2.1 (Binary is M.I.A)
	+ Recompiled fo KSP 1.2.1
	+ Code cleanup and bugs hunting. Some bugs removed some bugs added. I tried to do camera interface to becomes more friendly, providing small "tips what to do" in different situations and will not allowing situations that causing exceptions. Also, seems like FPS drop down, when many camera windows are opened, becomes significantly less.
	+ Restriction for turning on "docking camera" has been removed. Now you can turn on DocCam without active target. Also, without target selected, it will not show flight data on its screen.
	+ Hard dependence from Blizzy toolbar removed, you can call config window by pressing Alt+1.
	+ According to the received requests - "Forced Camera Shutdown" has been added. In config window you can select a swith and when camera window, which transmitted from the nonactive vessel, dissapears when nonactive vessel exits out of range it will or will not (depends of switch) appears again when non active vessel with camera will come back to range.
New camera window will be opened near previous, without overlapping each other.
	+ Do not forget that cameras needs electricity, and if it will be depleted, camera windows will be closed.
	+ Hope, all should work as expected, if not - feedback are welcomed
* 2016-1017: 1.2.0.2 (DennyTX) for KSP 1.2 (Binary is M.I.A)
	+ Fixed issue with dissapearing button panel.
	+ Electrisity consuption was back
* 2016-1011: 1.2.0.1 (DennyTX) for KSP 1.2 (Binary is M.I.A)
	+ Version file.
	+ recompiled for 1.2. release
	+ minor interface changing
* 2016-1009: 1.2 (DennyTX) FOR KSP 1.2 PRE RELEASE (Binary is M.I.A)
	+ KSP 1.2.pre ready.
	+ electricity consumption temporarily disabled.
	+ Added toolbar button.
	+ can change unload range.(via toolbar button)
	+ shaders divided to three groups (via toolbar button)
	+ added 2 new modes for cameras, installed on non-active vessels
* 2016-0609: 0.0.1.7 (DennyTX) for KSP 1.1.3 (Binary is M.I.A)
	+ moved auxiliary textures to assetbundle
	+ embedded six new shaders (see example)
	+ digital noise can be turned on/off  by toggle (and in cfg too)
	+ camera number and its target shown in window title
	+ reports whence being broadcast images, when the camera has been activated on the other (non-current) vessel and vessel has been changed (at distance less than 2500)
	+ many cameras can work simultaneously
	+ has been checked to 32- and 64 bit assemblies.
* 2016-0605: 0.0.1.6 (DennyTX) for KSP 1.1.2 PRE-RELEASE (Binary is M.I.A)
	+ Temp build. code cleanup for KSP 1.1.2
* 2016-0605: 0.0.1.5 (DennyTX) for KSP 1.1.2 PRE-RELEASE (Binary is M.I.A)
	+ Temp build. code cleanup for KSP 1.1.2
* 2015-1113: 0.0.1.4 (DennyTX) for KSP 1.0.5 (Binary is M.I.A)
	+ The target beam scanning with its own scientific experiment has been added. It triggered when certain conditions met. Namely - the need to focus the camera at the subject (chosen target) and irradiate it. If the range (set in CFG) are within a given (it accordingly may require a rapprochement with the object) - will be carried out the experiment. if the conditions are not met - will not. The experiment has a limit of (4 times) and consumes resources (configurable in CFG). Further development - something to do with the system of contracts that can be ordered reconnaissance flights.
	+ Saving screenshots has been added. It will be collected in a separate directory that is bound to the name of the game, with the time mark in the name. I think about video recording, but so far only with the external library. However, still not sure it needed.
	+ Additional zoom modes has been added. Optical zoom can be increase with coeff 10, as well as wide-angle camera mode.
	+ Target's tags has been added.
	+ Toggles for all interface elements has been added. Can be made by switchable toggles or through CFG.
	+ Helper cross in docking camera now support two modes of operation. First - my mode, second - duplicates the work of DockingPortAligmentIndicator.
	+ The initial window size can now be set through the CFG. Ie no longer necessary to have only default 256 points ( can be supplied, for example - 500, and then the following steps will change the scale coefficients to 1.5 and 2 (ie, get 750 and 1000 respectively).
	+ A lot of small fixes. Such as following: the new camera window will not overlap the time scale. Cameras informs about broadcast (useful, if the camera is turned at the currently inactive ship). Button for window close. Rebuild for 1.05.
* 2015-1107: 0.0.1.2 (DennyTX) for KSP 1.0.4 (Binary is M.I.A)
	+ Docking camera will get its position from "dockingNode" now, this should fix the problem with Inline Clamp-O-Tron.
	+ Color of "targetting cross" will be customizable in CFG.
	+ Most operational buttons has been moved in openable window.
	+ Flight data and roll rotator can be turned off/on by toggle.
	+ Flight data from cameras, that installed at other vessel (non current one) will be shut off.
	+ Bug with red text everywhere seems to be fixed. (deltaZ speed must become red only if closure rate becomes higher 3 m/s or if we moving away from the target).
	+ Speed of part-camera rotation by axiss becomes depending on the current zoom. High zoom - smaller step of rotation.
	+ More verifications has been added into the code.

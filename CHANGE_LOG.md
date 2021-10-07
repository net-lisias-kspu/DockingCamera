# Docking Camera (KURS) :: Change Log

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

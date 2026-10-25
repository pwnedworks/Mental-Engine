# Mental Engine
![logo](Logos/Mental_Engine_logo.png)
========================

**Mental Engine** is a fork of [**Serious Engine 1**](https://github.com/Croteam-official/Serious-Engine)



Building
--------

To build Mental Engine, you'll need [Visual Studio (from 2013), Professional or Community edition](https://www.visualstudio.com/post-download-vs?sku=community).

Do not use spaces in the path to the solution.

Once you've installed Visual Studio and (optionally) DirectX8 SDK, you can build the engine solution (`/Sources/All.sln`). Press F7 or Build -> Build solution. The libraries and executables will be put into `\Bin\` directory (or `\Bin\Debug\` if you are using the Debug configuration).

Running
-------

This version of the engine comes with a set of resources (`\SE1_10.GRO`) that allow you to freely use the engine without any additional resources required. However if you want to open or modify levels from Serious Sam Classic: The First Encounter or The Second Encounter (including most user-made levels), you will have to copy the game's resources (.GRO files) into the engine folder. You can buy the original games on Steam, as a part of a bundle with Serious Sam Revolution ( http://store.steampowered.com/app/227780 )

When running a selected project, make sure its project settings on Debugging is set to the right command:
* For debug:
    $(SolutionDir)..\Bin\Debug\$(TargetName).exe`
* For release:
    $(SolutionDir)..\Bin\$(TargetName).exe`
And its working directory:
    $(SolutionDir)..\

Common problems
---------------

Before starting the build process, make sure you have a "Temp" folder in your development directory. If it doesn't exist, create it.
SeriousSkaStudio has some issues with MFC windows that can prevent the main window from being displayed properly.

License
-------

Mental Engine is licensed under the [GNU GPL v2](https://github.com/pwnedworks/Mental-Engine/blob/master/LICENSE).

Some of the code included with the engine sources is not licensed under the GNU GPL v2:

* [zlib](https://github.com/madler/zlib) (located in `Sources/Engine/zlib`) by [Jean-loup Gailly and Mark Adler](https://github.com/madler)
* [LightWave SDK](https://lightwave3d.com/) (located in `Sources/LWSkaExporter/SDK`) by [NewTek Inc.](https://www.newtek.com/)
* [libogg/libvorbis](https://www.xiph.org/vorbis/) (located in `Sources/libogg` and `Sources/libvorbis`) by [Xiph.Org Foundation](https://www.xiph.org/)
* [libmpg123](https://github.com/gypified/libmpg123) by [gypified](https://github.com/gypified)

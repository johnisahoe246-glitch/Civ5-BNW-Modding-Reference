This page includes information on the Civ5 Modding Tools as well as links to other useful programs.

= SDK =
'''World Builder'''
:The stand-alone world builder allows users to create and modify maps and scenarios for Civilization V.

'''Mod Buddy'''
:An editor (IDE) for the XML and Lua elements of the game and allows for the creation, packaging, and uploading of mods. To use it, you have to install the [http://www.microsoft.com/downloads/en/details.aspx?FamilyID=DFBA7AC4-5366-456E-ABD6-0E3E6BA83B7C&displaylang=enMicrosoft Visual Studio 2010 Shell (Isolated) Redistributable Package]. ModBuddy will prompt you to install this if you don't have it already
:[http://forums.civfanatics.com/showthread.php?t=387554 Installing ModBuddy Extensions]

'''Nexus'''
:A collection of tools to to work with the art in Civilization V.
:[http://forums.civfanatics.com/showthread.php?t=386972 Initial Look at Nexus, 3D Unit Art, and Reskinning]
:Note that Photoshop templates for icons are also bundled in the SDK, under the ''Art'' folder (in ''Programs Files/Steam/...'').

'''FireTuner'''
:An advanced debugging terminal. It displays the lua output, provides an interactive console and can be simply extended with custom controls and tables.
:Do not forget to modify your *.ini files, see [[Debugging (Civ5)#Configuration|Debugging#Configuration]].
:[http://forums.civfanatics.com/showthread.php?t=399821 Simple Tuner Modifications]


= Digging the source code and the data tables =
Since the documentation is sparse, you need a tool to quickly inspect the civ5 source and data files and search in all of them at once. See also [http://forums.civfanatics.com/showthread.php?t=475076 this comparison of search tools].

'''Notepad++'''
:A great and renowned text editor with a "search in all files" feature (hit ctrl + shift + f). Used by many developers around the world. [http://sourceforge.net/projects/notepad-plus/ Download].

'''Visual C++ 2010 Express'''
:This is Microsoft's free C/C++ IDE, which is needed in order to compile the DLL. It includes code editing, autocompletion, compilation, and debugging and can be downloaded [https://www.microsoft.com/visualstudio/eng/downloads#d-2010-express here]. NOTE: any more modern version of Visual Studio should work so long as you have VC++ 2010 installed as well.

= Browsing the art assets =
'''Dragon unpacker'''
:Can extract the Firaxis packages (.fpk files). [http://sourceforge.net/projects/dragonunpacker/ Download].

'''DDS Unpacker'''
:Some DDS files have been compressed even further and look messed up if you open them in an image viewer. This tool rebuilds them. [http://forums.civfanatics.com/showthread.php?t=389316 Download].

'''XnView'''
:An images browser to get a quick look at all the DDS files to spot the one you're looking for. [http://www.xnview.com/en/download.html Download].

'''FireTuner: Textures Viewer'''
:A FireTuner panel to browse most of the game's textures. [http://forums.2kgames.com/showthread.php?118165-MOD-LiveTuner-Texture-Viewer Download].

'''FireTuner: Icons Viewer'''
:A FireTuner panel to browse the game's icons. [http://forums.2kgames.com/showthread.php?118055-MOD-LiveTuner-Icon-Viewer Download].


= Creating Art Assets =
'''NVidia Texture Tools for Photoshop'''
:A Photoshop plugin to save textures under the DDS format. [http://developer.nvidia.com/content/nvidia-texture-tools-adobe-photoshop Download]

'''Paint.net'''
:An easy-to-use and moderately powerful open-source image editor for Windows that natively supports the DDS format. [http://www.getpaint.net/ Download]

'''GIMP'''
:A free & open source image editing and manipulation tool. Very useful for creating 2d assets (icons). A windows installer version can be downloaded [http://www.gimp.org/downloads/ here].

'''Nexus Buddy 2'''
:Created by a member of the CFC community, this tool makes it much easier to work with 3d assets, especially for things other than units. You can download the latest version from the forums [http://forums.civfanatics.com/showthread.php?t=496855 here], and it is actively updated by its author.

= Testing and debugging =

=== SQLite tools ===
Anytime it starts a game, Civilization V saves a SQLite snapshot of the database, including the changes made by mods, under ''Civ5DebugDatabase.db''. 

'''SQLite Manager'''
:NOTE: This is at the moment not compatible with the latest version of Firefox. The latest version it is compatible with is 19.0. 
A Firefox plug-in, slightly more powerful than the previous tool. [https://addons.mozilla.org/en-US/firefox/addon/sqlite-manager/ Download]

'''SQLiteSpy'''
:A Windows software to inspect the SQLite files. [http://www.yunqa.de/delphi/doku.php/products/sqlitespy/index Download]

'''SQLite Browser'''
:A Windows software to inspect the SQLite files. [http://sqlitebrowser.sourceforge.net/screenshots.html Download]

=== Cheating tools and game inspectors ===
'''In-game Editor (IGE)'''
:Add or remove units, cities, resources, change the terrain, trigger wars, etc. Convenient to quickly test your mod. [http://forums.civfanatics.com/showthread.php?t=436912 Download] (also on the Steam Workshop).

'''FireTuner: Techs and policies panel'''
:A FireTuner panel to list, grant and revoke techs and policies. [http://forums.2kgames.com/showthread.php?108533-MOD-LiveTuner-Tech-and-Policy-Panels Download].


[[Category:Civ5]]
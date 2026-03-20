= General =
MapView is a Worldbuilder like application that allows the creating and modification of scenarios and maps for basicly all different tastes of Civilization 4. By today, Februaray 9th 2011, the most recent version is 2.0.9.

This article is about MapView 2 mainly. It might contain information about MapView 1 (Version 0.x) but will not give you hints or tips about MapView 1 can be used since it is considered deprecated.

= Download & Main Thread =
The direct download link can be found in the [http://forums.civfanatics.com/downloads.php?do=file&id=11554 Civfanatics.com download section]. 
The official thread of the application can be found [http://forums.civfanatics.com/showthread.php?t=305168 here].

=== Older versions ===
* [http://www.weown.de/files/MapView/MapView-2.0.9.zip 2.0.9]
* [http://www.weown.de/files/MapView/MapView-2.0.8.zip 2.0.8]
* [http://www.weown.de/files/MapView/MapView-2.0.7.zip 2.0.7]
* [http://www.weown.de/files/MapView/MapView-2.0.6.zip 2.0.6]
* [http://www.weown.de/files/MapView/MapView-2.0.5.zip 2.0.5]
* [http://www.weown.de/files/MapView/MapView-2.0.4.zip 2.0.4]
* [http://www.weown.de/files/MapView/MapView-2.0.3.zip 2.0.3]
* [http://www.weown.de/files/MapView/MapView-2.0.2.zip 2.0.2]
= Upcoming Changes =
The development of MapView is currently on hold. I've been working on the promised changes but couldn't find the time to roll out a release yet. I actually do minor work on the project but it doesn't really look like i'll release a new version soon.

The Version currently in development contains the following changes.
* Removed Copy Paste, Selection, Deselection etc. (It's a plugin now)
* Added CopyPasteEtc. Plugin witch will now overtake what the main app did
* The "New Map" Dialog finally shows the buttons by default
* The "New Map" Dialog has now default values "100x100"
* Changed Kernel to be a singleton class
* Renderer now uses VBOs if available, should increase render performance quite a bit
* Added Script Plugin .. Simple python interface for now
* Exposed some basic API Classes to Python
* Started working on a dynamic Pic2Map Version, fixed resolution sucks
* Improved Pic2Map to allow the User to enter the desired map dimensions
* City Names can now be shown in View (Toggle over Render Menu)
* Some more internal changes. STL output will now log to the application log windows
* In some cases changing Mods could get stuck in an infinite loop. Thx to Beezle for that find.
* Pen Tool will now show on which size your work (just for terrain atm. ignore for anything else)
* Unknown Lines will be saved .. that will basicly open up support for anything. Next step is to give you an option wether or not this unknown lines will also be saved.

= Features =

== Feature Briefing ==
MapView is able to edit almost every part of a given scenario file, as long as the keywords inside the file is according to [[Vanilla]], [[Warlords]] or [[Beyond the Sword]]. 
For example, Version 2.0.7 cannot operate with settings like "EuropeType" that is used in [[Civilization 4 - Colonization]] . But, no worries. That's no reason you can't use MapView at all. You will usually be able to create your map as usual and then edit the complete map to contain the necessary keyords after you are done with the basic setup.
It's probably recomendet to use tools like [http://www.winmerge.org/ Winmerge] to simplify the use of MapView together with unsupported keywords.

== Key Features ==

* Create and save Maps up to a size of 400 x 400 tiles
* OpenGL View
* Zoom and Pan
* Buttons for all common things
** Terrain Types
** Feature Types
** Bonus Types
** Route Types
** Units
** Cities
** All those can be unique for your personal mod (see 'Support for custom mods' below)
* Toolbars for intuitive work
* Support for custom mods
** Learns from the Mod's *.xml files
** Dynamic GUI and OpenGL rendering to allow visual representation for your mod's unique boni etc.
* Basic Workflow
** Create & delete
*** Terrain
*** Bonus
*** Features
*** Cities
**** Wonders
**** Buildings
*** Units
**** Owner 
**** Promotions *.etc
*** Routes
*** Rivers
* Tools
** Floodfill
** Pen
** Eraser
** Copy, Cut & Paste
* Layer System
* Team Reveal
* Plugin Support (C++ but SDK yet to be released)

= FAQ - Frequently asked questions =

Here you can find a list of frequently asked questions.
=== Maps (BTS, mayb others too) created with MapView crash ===
Read [http://forums.civfanatics.com/showpost.php?p=8601140&postcount=230 this] and [http://forums.civfanatics.com/showthread.php?p=8881786#post8881786 this] to learn what causes this problems. Also have a look arround the pages [http://forums.civfanatics.com/showthread.php?t=305168&page=9 9], [http://forums.civfanatics.com/showthread.php?t=305168&page=10 10], [http://forums.civfanatics.com/showthread.php?t=305168&page=11 11] and [http://forums.civfanatics.com/showthread.php?t=305168&page=12 12] of the MapView Mainthread to find out more about this issue. A few valuable links and threads are mentioned. Also, feel free to enhance this article according to any issue you solved. Also have a look at the next solution in this FAQ.

=== Civ Crashes when i try to load the scenario i made ===
Especially for, but not limited to, BTS and BTS Mods this might be common. The BeginPlayer/EndPlayer parts in the scenario files are not saved properly. A few things might need to be changed. You need to set the Handycap and other things. Look at [http://forums.civfanatics.com/showthread.php?p=8395570#post8395609 this thread] where someone had a the similar problem. The best way to solve this is using [http://winmerge.org/ WinMerge] and compare a working file with the file MapView created and try to fix proplematic areas. 
The next Version (2.10) will fix some of the problems.

=== How to move the view or zoom? ===
Press and Hold the 'Space'-Key then press the left mouse button to move or the right button to zoom. The mousewheel should also allow you to scroll. 

If this does not work for some reason, press the "Mouse" Button in the Toolbar. (The big mouse pointer image). After you pressed it you should be able to navigate as explained above

=== MapView crashes when i load a map ===
This should NOT happen. If the map works fine in Civilization, please let me know.

=== MapView crashes when i change to a certain Mod ===
Since MapView learns from the xml files that come with any mod it's very likly that something went wrong while MapView parsed those files. I still have to come up with a more clever way to handle this. Please report such behavior in the main thread and provide a link to the mod so i can try on my own. 

=== MapView crashes when the application starts ===
If you are using the Editor Version that came with MapView it's very likly that you modified something in the xml files that come with Vanilla. 

=== How to work mod depending? ===
Go to 'Plugins' -> 'Editor' -> 'Mods' and find and select the Mod you want to work with. After selection, the mods xml files will be parsed and the toolbars will be re-filled with all available data. You will probably see A LOT of question marks after loading an unofficial mod.

=== My toolbars are full of question marks ... why? ===
MapView get's it's knowledge from the xml files that define the content and behavior of a mod. Whenever MapView can't display an image for a certain bonus, feature, etc. it will display a question mark. If you want to, you could create your own image to get MapView to show a nice little image. (See Video Tutorials)
 
=== My map view is full of question marks ... why? ===
See: 'My toolbars are full of question marks ... why?'. It's the same reason, just for the OpenGL renderer.

=== I want to edit the TeamReveal, where are the functions? ===
When you right click on the Team Reveal Button you get a drop down box that let's you chose from several advanced ways to handle team reveal for the selected player.

=== How to delete Cities or Units? ===
Whenever you click on a field that contains a city or units the 'Tile Inspector' will show those. You can right click on the City or Unit Nodes and delete it from there. Units can also be deleted by pressing the delete key on your keyboard.

=== How do i delete a River/parts of a river? ===
Make sure you have the river editing tool selected. Press and hold down the right mouse button and move the mouse over the fields where you want to delete the river fields.
You can also delete whole rivers from source to mouth by pressing shift, and the left clicking on a river.

=== I want to use Pic2Map Plugin with another Map size ===
Currently the dimensions are hardcoded so you need to trick the plugin to get to the goal. To learn how, look [[#Map Size|here]].
'''Update''' 2.0.10 will allow you to define the size.

=== Can i use MapView on Computers that don't have Civ installed? ===
Yes, of course. MapView basicly looks up the Mods folders of Civ, Bts and Warlords and will learn from the "Assets/xml" folder that is available in those game-types. In Short words: If you make a copy of your Civ folder and delete everything that is not an xml file, you will have a small, reduced version of Civilization that can be transfered to any other computer and act as a "Civilization 4" emulator for MapView. Check the File Menu for the overwrite option.

= Python/Script FAQ - Help =
Version 2.10 will allow you to run custom python scripts that will allow a lot of things to be changed by script. This section is intended to supply a decent overview of how this works. I hope i can get a decent documentation and a lot of examples done so you can learn about it easily. MapView 2.10 will ship with 10+ example scripts that will get you started. There's already a little article about it available [[MapView Python | here]].

= Plugins = 
Most of the features in MapView are realized as plugin. Those plugins can be found in the main application folder. You can identify them by the filename that is something like 'plug_<name>.dll'. Without any of those plugins, MapView will still let you view a map but all other features are very limited. Most of the really useful things are parts of the editor.

== Editor ==
* Purpose:  most editing functionality
* Current Version: 1.3.1

== CreateCoast ==
* Purpose:  advanced coast features
* Current Version: 1.0
* Author: GreyHound

== Remover ==
* Purpose: advanced removing capabilities
* Current Version: 1.0
* Author: GreyHound

== RiverPlace ==
* Purpose: adds functionality to place and delete rivers
* Current Version: 1.0
* Author: GreyHound

== TileToText ==
* Purpose: previews how a certain tile will look after saving (this might be a little inaccurate since i made changes to the saving algorythm depending on the file extension, but it will basicly be correct)
* Current Version: 1.0
* Author: GreyHound

== LandscapePlacer ==
* Purpose: let's you place hills, peaks, flatlands and below sealevel
* Current Version: 1.2
* Author: GreyHound

== TeamReveal ==
* Purpose:  for teamreveal editing
* Current Version: 1.0
* Author: GreyHound

== Pic2map ==
* Purpose:  converts Images to maps
* Current Version: 1.0
* Author: GreyHound

Pic2map offers the opportunity to take a picture. (A satellite photo or such) and generate the basic continent shape with accurate terrain matching easily. It works best with JPG files, bmp has often given bad results.
=== Map Size ===
'''UPDATE:''' MapView 2.0.10 will allow to define the size via Gui. 

Currently the size of the generated map is hardcoded but you can trick the plugin to generate other mapsizes too. I'll explain how this works. 
Remember, the whole image will currently represent a 130 x Y sized map. (Y is adjusted to fit the src picture aspect ratio, a 100 x 100 px source generates 130x130, 100x50 px generates 130 x 65 etc. ). This example shows how to get a map with 65 tiles in width.

# Open your source image with an image editor.
# Resize the CANVAS to 200% x 200% (Don't scale the image, just enlarge the working area)
# Your image now consumes the same amount of pixels as before but relativly to the image size it's only half the size. 
# Use the new picture in MapView and generate a map.
# Select and Copy the relevant part of the generated map.
# Create a new map (should be 65 x Y/2 in this example) and paste the copied area.
# Be Happy ;D

With this system you can basicly get any size you want to.

= History =

The first Version of MapView was released November 17th, 2005 and has been downloaded arround 10000 times. Due to the lack of features and horrible programming a new Version was released January 6th 2009. It has had arround 9500 downloads by November 17th, 2010.

== Versions == 
[http://forums.civfanatics.com/showthread.php?t=305168 MapView 2.x official Thread]
[http://forums.civfanatics.com/downloads.php?do=file&id=11554 MapView 2.x official Download]

[http://forums.civfanatics.com/showthread.php?t=141622 MapView 0.x official Thread]
[http://forums.civfanatics.com/downloads.php?do=file&id=4539 MapView 0.x official Download]

== Motivation ==
The first version, written in 2005 was highly inspired with Junuxx's application [[Atlas]]. The first intention was to create an application that let's you look at a scenario without having to start Civilization, thus, save time. That's also the origin of the applications name. It's been designed to let you 'view' a map. By the time features were added until MapView became an editor for WorldBuilderSave files.

I had a few attempts in rewritting MapView from 2006 to 2008 but always stopped halfway through. In Autumn 2008, when i had one month off i finally pushed out another version.

= Used libraries =
'''MapView'''
* Forgot
'''MapView 2'''
* [http://openil.sourceforge.net/ DevIL 1.7.8] (Image library)
* [http://www.wxwidgets.org/ wxWidgets 2.8.9] (GUI)
* [http://freetype.sourceforge.net/ FreeType 2]
* [http://www.grinninglizard.com/tinyxml/ TinyXML] (parsing)
'''MapView 3 (in development)'''
* [http://openil.sourceforge.net/ DevIL 1.7.8] (Image library)
* [http://qt.nokoa.org/ QT 4.6.1] (GUI, XML)
[[Category:Civ4 Map Editors]]
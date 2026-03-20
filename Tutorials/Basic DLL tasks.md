=Basic DLL Tasks=

The Civilization V SDK ships with the C++ source code for the Civilization V CvGameCoreDLL. This is the most powerful tool modders have, as it allows us to directly alter game code and game logic, but also one of the least used, as it has a codebase in excess of 100,000 lines of code and the architecture of the program is not always clear. In this article some basic tasks in modding the DLL will be covered, as well as some more advanced ones as well.

=Requirements=

This article is NOT a C++ tutorial. If you need one of those, Google is your friend. I will assume that you have knowledge of C++ coding, as well as knowledge of how a civ game works. I will not assume knowledge of the Civ 5 dll or the civ 4 dll, which was very similar architecture-wise.

=Compiling the DLL=

The DLL source comes with solutions for Visual Studio 2008, 2010, and 2012 (the 2012 one also compiles in 2013). However the project requires the VC++ 2008 toolchain. Since Visual Studio 2008 is a slightly outdated IDE it doesn't have the best features, so you should install Visual C++ 2008 Express and Visual C++ 2013 express to get the best development experience. If you don't want to do that just developing in VC2008 is fine as well. Any of the paid versions of Visual studio from these years will also work. Both of the express ones can be downloaded for free from Microsoft's website.

Once you have your IDE(s) installed you only need to make one change to make the DLL compile. In CvGameCoreDLL.rc for each project (there are 3, one for each dll) you need to change the reference to afxres.h to windows.h. After this simply build (you may need to clean first) and you should get 3 dlls, one for vanilla, G&K, and BNW. Note, you can safely remove the projects for versions your mod will not support (ie, you can only have it build the BNW dll).

To add a new DLL to a mod, open up ModBuddy, and right click your mod project and select 'Add existing item'. Navigate to the output folder from Visual Studio and select the DLL file, then click 'add'. After this you need to set import to VFS for true for the DLL, and when your mod loads it should also tell the Civilization 5 exe to unload the normal DLL and load yours.

=Basic Civ 5 DLL Architecture=

The civilization 5 DLL has a lot of code in it and can be confusing to a newcomer. In this section I will endeavor to give a 30000 foot overview of the internals of the DLL.

The Game Objects: The Civilization 5 game is represented by a few major classes. 

'''CvGame:''' This class is the current game in progress. It contains basic info about the game, such as the settings used to create the game. It also does game-level things such as track score and check for winners, among other things.

'''CvMap:''' This class contains the game map. It contains all of the CvPlots, as well as map-wide methods, such as the areas visible, the areas which contain water, the number of owned plots, etc.

'''CvPlot:''' This is one hex tile in the game map. It contains enough data to describe what it is (terrain, features, improvements, resources, etc). It is also referenced by all location-based game objects and functions, so if you are making any edits to location based game mechanics you will need to edit CvPlot to be aware of these mechanics.

'''CvPlayer:''' This is a human or AI player. If AI, it owns all of the AI objects. NOTE: Any player-wide effects you want to add should normally be handled through CvTeam, which deals with permanent allies and other instances of multiple civs working together. CvPlayer should only be used if you want to expressly want the effect to only be on one civ. 

'''CvCity:''' This is one city. It (through other objects) handles all buildings inside it, and processes many different effects. It also is responsible for ensuring that construction of anything is properly handled. 

'''CvUnit:''' This is a unit. It mainly contains info about itself and it's situation. It is also responsible for moving itself around and performing actions on it's environment. It is NOT responsible for combat. See CvUnitCombat if you really want to mess with combat mechanics.

These are far from the only objects, and each of these objects is more complex than this. This is only meant as a top-level overview for new dll coders on where to go if you want to do certain things. Later I will explain how these interact with the data loading code when I write about new XML/SQL items.

=Creating a new boolean XML tag/SQL column=

Coming Soon...

=Creating a new integer/floating point value XML tag/SQL column=

Coming Soon...

=Creating a new multi-level XML tag/SQL column=

Coming Soon...

=Debugging your custom DLL=

Coming Soon...

=Advanced Tips and Tricks=

Coming Soon...
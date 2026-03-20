''This page is a part of the [[Civ5 Modding Tutorials]].''

This article explains the Virtual File System (VFS) in Civ5. Lua developers looking for informations on the '''include''' function should look at [[Specificities of the Lua implementation in Civ5]].


= What is it? =
[[File:ModBuddy.ImportIntoVFS.png|frame|The ''import into VFS'' option.]] 
VFS stands for Virtual File System. Rather than locating the files directly in the file system, Civ5 looks for them in its virtual file system. This system provides the following benefits:
* '''Modularity:''' each mod, expansion or DLC can provide its own version of a given file without overwriting the original one. At run-time the game sequentially loads those files into the VFS, performing virtual overwrites as needed. This contrasts with the mods hell in the Elders Scrolls series for example.
* '''Packaging:''' The files in the VFS can be either independent files or parts of packages (archives). The VFS behaves as a unified resource loader.
* '''Sandboxing:''' whenever a mod requests a file, civ5 only looks in the VFS. This prevents mods to be allowed to look at the physical file system since this could open a security breach.


= Determining whether a file must be imported or not =
In doubt, import your files into the VFS. But you should better stick to what is written here.


'''Must be imported''' the files that are requested during the game.
* The XML UI files. 
* The XML files for animations, scenes, etc.
* The Lua files (minus the exception detailed below).
* The art assets such as textures or models.


'''Should not be imported''' the files that are loaded through the project's content and actions tab (except the XML UI files, those ones should always be imported). While this is harmless most of the time, this can sometimes result in unexpected side-effects.
* The Lua files that are directly loaded through the project's content tab. This does not apply if the Lua file is associated with a XML file and you load this XML file instead. Note that if you want a Lua file to be included by other Lua or XML UI files, you will still have to import it into the VFS but you may see it loaded more times than necessary. 
* The XML data and text files. Those ones are only ran at start up to modify the data tables.
* The SQL files. For the same reasons.


= Importing a file into the VFS =
* In ModBuddy, select a file in the solution explorer. 
* Hit F4 (or click View > Properties Window) to open its properties.
* At the bottom of this new window, look for '''Import into VFS''' and set it to true.
* If Civ5 is opened, you will need to exit to the main menu for this change to be applied.


= Final warning =
{{Warning}} In some circumstances (notable the include statement in Lua, see [[Specificities of the Lua implementation in Civ5]]) only the first eight characters of the file matter. Tow files starting with the same first eight characters could then be confused by the game.


[[Category:Civ5 Tutorials]]
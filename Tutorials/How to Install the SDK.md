These instructions were originally compiled by [http://forums.civfanatics.com/downloads.php?do=file&id=10018 Refar] for Visual Studio 2005, and have since been slightly modified for a newer version of the Makefile.  They will also work with Visual Studio 2008 and 2010. They assume the modder is compiling the Beyond the Sword (BTS) DLL.

Once you have the SDK installed, you'll probably want to look at Xienwof's [http://forums.civfanatics.com/showthread.php?t=314201 An Idiot's Guide to Editing the DLL] to get started with editing the SDK.

==Installing the Tools==
* Download and install [http://kael.civfanatics.net/files/VCToolkitSetup.exe Microsoft Visual C++ Toolkit 2003]
* Download the following three library files and put them in this folder: C:\Program Files\Microsoft Visual C++ Toolkit 2003\lib
** [http://kael.civfanatics.net/files/msvcrt.lib msvcrt.lib]
** [http://kael.civfanatics.net/files/msvcrtd.lib msvcrtd.lib]
** [http://kael.civfanatics.net/files/msvcprt.lib msvcprt.lib]
* Download and install [http://msdn.microsoft.com/vstudio/express/visualc/download/ Microsoft Visual C++ Express Edition]
* Download Makefile.7z from [http://forums.civfanatics.com/showthread.php?t=370861 this forum thread] and unzip it. You don't need to do anything with it yet.

* Download and install the [http://kael.civfanatics.net/files/PSDK-x86.exe Microsoft Platform SDK]

==Preparing the Working Folder==
Compiling a Civilization 4 DLL requires you to use the BtS source files as a base. To begin with locate the CvGameCoreDLL folder; it can be found in your main Beyond the Sword folder (if it is not there, you need to re-install your copy of BtS).  Copy this folder to a working directory so that you maintain the original BtS source files in their original location, and have a separate development directory to work from.  It is highly recommended that you first compile a clean BtS DLL using only the source files in the CvGameCoreDLL folder before editing the source, or merging in source from other mods.

* Remember: make a copy of the CvGameCoreDLL folder to work with (including its subfolders) and put this copy in a location where you want to keep your working files.  '''From now on everything said refers to the working copy of the files. ''Don't ever modify the original files – you might need them''.'''
* Delete the files CvGameCoreDLL.vcproj and CvGameCoreDLL.rc.  ''If you followed the instructions so far (i.e. are using a clean copy of the SDK files released with a patched version of BTS) these 2 are all you need to delete.  If however your sources came with a mod or were edited with other programs before, there might be a few more files to get rid of. These might be: CvGameCoreDLL.vcproj.vspcc, CvGameCoreDLL.ncb, *.sln, and perhaps others.  The only files you need are: All *.h files, all *.cpp files, all (2) *.inl files and everything in the both subfolders (You don’t need to touch the subfolders at all).''
* Put the makefile from Makefile.7z into your working folder.  The Makefile should work for all versions of Civ, including Colonization, with no modifications.
* Open the Makefile in your preferred editor. You can use the freshly installed Visual Studio IDE, or something else if you prefer.  ''Windows Notepad does not work well here.''
* At the very top, change the line that begins with TOOLKIT to the path of your Visual C++ Toolkit 2003 directory.
* Change the line that begins with PSDK to the path of your Microsoft Platform SDK.
* Optionally, uncomment the line beginning with "YOURMOD" to point to your mod's directory. This will automatically copy the DLL to your mod's Assets directory.
* Save the Makefile and exit.

==Setting up the Project==
Launch the IDE.  When setting up the project for the first time, do not open the existing project file in Visual C++ Express Edition.  ''In fact, if you followed so far, there should be no project file right now.  When compiling the same project for the second, 3rd,… time, you do not need to repeat all the steps – you can then load the project file you will create when you are through with this instructions.''

* Click  -File- -New- -Project-. The "New Project" window will open.
* In the "Project types" box select  –General-. In the "Templates" box select -Makefile Project-.
* In the "Name" box type "CvGameCoreDLL".
* In the "Location" box browse to the folder where you copied your CvGameCoreDLL folder to. This folder MUST be the last folder listed in this box. For example, if you copied CvGameCoreDLL to another folder like so:  C:\MyModsFolder\CvGameCoreDLL , then the entry in the "Location" box must read: C:\MyModsFolder
* UNCHECK the box that says "Create Directory for Solution".
* Click -OK-. The "Makefile Application Wizard" will open.  Click –Next-. Clear all the boxes. Click –Finish-.

You will see the IDE interface now, showing you a yet empty project. To avoid possible errors in VS 2010, we will first configure the compiler, and then add source files.

* Click -Project- -CvGameCoreDLL Properties-. The "CvGameCoreDLL Properties Pages" window will open.
* In the left-hand box under "Configuration Properties" select "NMake". ''Previous versions of the makefile required you to change the configuration properties here. The newer makefile does not require you to do so.''

* Select the "Release" configuration from the "Configuration:" drop-down-box in the top left corner.
* In the right-hand box under "General" it says "Build Command Line". Click the empty box to the right of it and type nmake Release.
* In the next line down, to the right of where it says "Rebuild All Command Line", click in the empty box and then click the button in the box at the right. The "Rebuild All Command Line" window will open. Type  nmake Release_clean, and then directly below it on a second line, type nmake Release. Click -OK-.
* In the next line down, to the right of where it says "Clean Command Line", type nmake Release_clean.
* Select the "Debug" configuration from the "Configuration:" drop-down-box in the top left corner, and repeat the 3 steps above for Debug.  '''Note the underscores in the clean command.'''

Close the configuration windows with –OK-. Now, we'll add the source files to the project.

* Click -Project- -Add Existing Item…-. The "Add Existing Item – CvGameCoreDLL" window will open. This folder will contain all of the source code files, the Boost-1.32.0 folder, and the Python24 folder.  Select everything (use Ctrl-A) and click -Add-.  ''You only want to add: all *.h files, all (2) *.inl files, all *.cpp files and the both subfolders. If you followed the instructions so far (i.e. deleted all unneeded files) CTRL+A will give you exactly this. If you – for whatever reason – kept some of the unneeded files, you need to deselect them manually.''

Save your Project. It will create a new CvGameCoreDLL.vcproj file, which you can open later. It will have your settings saved.

You are done now. For a test you should compile the unchanged code under both Configurations (It takes a bit of time depending on your Hardware), to make sure everything does work as expected. You should use Build->Build Solution to do that.

==Compiling the Command Prompt==
You can also compile the project by invoking nmake from the command prompt. This might be useful if you repeatedly fail to get the configurations right, or if you want to quickly compile a 3rd party project without going through all the configurations steps. (You still need to install all the tools).

Run the Visual Studio IDE. Do not load a project (or do so – it doesn’t matter here). From menu select  Tools->Visual Studio Command Prompt. A console window will open. It has all the needed environment variables set properly (as opposed the usual command prompt Windows will give you).

Navigate to the folder where your project is (Using cd …).  Type:  nmake /f Makefile Final_Release to compile the final Release configuration. You can use another target instead, nmake /f Makefile Clean_Debug for example.

==Compiling a Single Source File==
Compiling a single file is much faster than building a full project. It does of course give you nothing actually run-able, but might still be useful when searching for code mistakes.

I did not find a way to do it from the IDE interface, but you can compile single files by invoking nmake from the console – as described above - and calling for intermediate targets.

nmake Debug/CvUnit.obj  
nmake Final_Release/CvUnit.obj  
for example will compile just CvUnit.cpp in the Debug or Final_Release configuration.

==Running the Debugger==
After compiling your project in the Debug configuration, you can run the game using the Debug-able CvGameCoreDLL.dll. It is a good deal bigger than your normal DLL and there is also a big CVGameCoreDLL.pdb file coming with it, which will contain information the debugger might need.

Start the IDE; load your project as switch to the debug configuration. Start the Game with the Debug-DLL.

I recommend running Civ4 Windowed; otherwise you might not be able to access the IDE after the game freezes on a breakpoint.

Choose  Debug->Attach To Process… from the menu. Choose the Civ4 Process. You might need to re-enable some local Services – for inexplicable reasons on XP debugging with Visual Studio Express does require Terminal Services to be running. In the debugger output window you will see the List of Libraries loaded in the Process. Most of them will say "No Symbols Loaded". This is fine. We are going to debug our CvGameCoreDLL.dll, so this is the only one we need symbols for.

Now you can debug. For testing set a Break-point on some function. CvGame::DoHolyCity() works fine – it is called once per turn. When the Game reaches the Breakpoint it will freeze waiting for your debugging action.

Another good test is a break-point at CvUnit::GetExperience(). When the game stops there, you can access the memory of the Unit instance that called the method and change its Experience level. The unit should be promoted on the next turn.
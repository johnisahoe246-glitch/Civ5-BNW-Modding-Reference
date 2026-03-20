The '''CvGameCoreDLLUndefNew''' file removes definitions for new, malloc, realloc, _msize, and free if USE_MEMMANAGER is defined. This is only defined if you are compiling a Debug DLL. CvGameCoreDLL then overrides them with what seem to be pure virtual functions.

The SDK is written in C++ and divided between header files (.h) and source files (.cpp). The header files contain all the unique classes used for Civ4; you will probably not be adding any new classes. They also hold lists of all the functions in the corresponding .cpp files, and their parameters. These files are divided into public, private, and protected areas, with variables and functions listed in each. The source files hold all the functions and the code - the meat of the SDK. Toying around with these will change AI behavior and let you mod the 'basic' parts of the game - sliders, traits, city structure, tiles, etc. 
<font color=red>This page is missing information.
Do not remove this notice until it is complete.</font>

{{Civ4_SDK_Files}}
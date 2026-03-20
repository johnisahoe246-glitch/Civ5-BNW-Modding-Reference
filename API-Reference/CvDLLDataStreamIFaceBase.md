The '''CVDLLDataStreamlFaceBase''' file appears to do nothing as it only has a #pragma once in it

The SDK is written in C++ and divided between header files (.h) and source files (.cpp). The header files contain all the unique classes used for Civ4; you will probably not be adding any new classes. They also hold lists of all the functions in the corresponding .cpp files, and their parameters. These files are divided into public, private, and protected areas, with variables and functions listed in each. The source files hold all the functions and the code - the meat of the SDK. Toying around with these will change AI behavior and let you mod the 'basic' parts of the game - sliders, traits, city structure, tiles, etc. 
<font color=red>This page is missing information.
Do not remove this notice until it is complete.</font>

{{Civ4_SDK_Files}}
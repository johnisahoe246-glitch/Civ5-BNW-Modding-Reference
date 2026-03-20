The '''CvHallOfFameInfo''' file handles getting the replay information for the hall of fame page of the main menu

The SDK is written in C++ and divided between header files (.h) and source files (.cpp). The header files contain all the unique classes used for Civ4; you will probably not be adding any new classes. They also hold lists of all the functions in the corresponding .cpp files, and their parameters. These files are divided into public, private, and protected areas, with variables and functions listed in each. The source files hold all the functions and the code - the meat of the SDK. Toying around with these will change AI behavior and let you mod the 'basic' parts of the game - sliders, traits, city structure, tiles, etc. 
<font color=red>This page is missing information.
Do not remove this notice until it is complete.</font>

==Functions==

Below is a list of all the functions in the file. Each function has a quick description attached to it. Note that there are comments strewn throughout some of these files, direct from the developers in order to aid the potential modders. All these functions are in the class CvHallOfFameInfo.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Function 
! style="background:#efefef;" | Parameters
! style="background:#efefef;" | Return Type 
! style="background:#efefef;" | Description
|-
!CvHallOfFameInfo::CvHallOfFameInfo()
|None
|Void
|Does nothing.
|-
!CvHallOfFameInfo::~CvHallOfFameInfo()
|None
|Void
|Runs SAFE_DELETE on every member of m_aReplays to clear up the memory used
|-
!CvHallOfFameInfo::loadReplays()
|None
|Void
|Loads the vector m_aReplays with ReplaysInfos through the loadReplays function of the CvDLLUtilityIFaceBase class. 
|-
!CvHallOfFameInfo::getNumGames() const
|None
|Integer
|Returns how many replays there are in the vector m_aReplays
|-
!CvHallOfFameInfo::getReplayInfo()
|int i
|CvReplayInfo*
|Returns the ith member of m_aReplays. Does not check to make sure it is in range.
|}

{{Civ4_SDK_Files}}
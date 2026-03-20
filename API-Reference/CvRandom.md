The '''CvRandom''' file handles generating random numbers and serializing them

The SDK is written in C++ and divided between header files (.h) and source files (.cpp). The header files contain all the unique classes used for Civ4; you will probably not be adding any new classes. They also hold lists of all the functions in the corresponding .cpp files, and their parameters. These files are divided into public, private, and protected areas, with variables and functions listed in each. The source files hold all the functions and the code - the meat of the SDK. Toying around with these will change AI behavior and let you mod the 'basic' parts of the game - sliders, traits, city structure, tiles, etc. 

<font color=red>This page is missing information. Do not remove this notice until it is complete.</font>

==Functions==

Below is a list of all the functions in the file. Each function has a quick description attached to it. Note that there are comments strewn throughout some of these files, direct from the developers in order to aid the potential modders. All these functions are in the class CvRandom.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Function 
! style="background:#efefef;" | Parameters
! style="background:#efefef;" | Return Type 
! style="background:#efefef;" | Description
|-
!CvRandom::CvRandom()
|None
|Void
|Calls reset without a defined value for ulSeed making it zero
|-
!CvRandom::CvRandom()
|None
|Void
|Calls uninit which does nothing
|-
!CvRandom::init()
|Unsigned long ulSeed
|Void
|Restores the value of m_ulRandomSeed to ulSeed
|-
!CvRandom::uninit()
|None
|Void
|Does nothing and is called with reset and the destructor
|-
!CvRandom::reset()
|Unsigned long ulSeed
|Void
|Calls uninit before doing anything and then sets m_ulRandomSeed to ulSeed if ulSeed is not passed sets it to zero.
|-
!CvRandom::get()
|Unsigned short usNum, const TCHAR* pszLog
|Unsigned short
|If logging is enabled it writes the current seed and turn slice to the log. It then does a set transformation to m_ulRandomSeed before doing a set of bitwise operations to return a semi random unsigned short
|-
!CvRandom::getFloat()
|None
|Float
|Returns the result of get with usNum as the largest unsigned short divided by the largest unsigned short each of which are made into floats prior to the division
|-
!CvRandom::reseed()
|Unsigned long ulNewValue
|Void
|Resets m_ulRandomSeed to ulNewValue
|-
!CvRandom::getSeed()
|None
|Unsigned long
|Returns the current m_ulRandomSeed
|-
!CvRandom::read()
|FDataStreamBase* pStream
|Void
|Calls reset and then reads a value from pStream to m_ulRandomSeed
|-
!CvRandom::write()
|FDataStreamBase* pStream
|Void
|Writes m_ulRandomSeed to pStream
|}

{{Civ4_SDK_Files}}
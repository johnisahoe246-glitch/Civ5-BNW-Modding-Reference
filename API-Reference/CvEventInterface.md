The '''CvEventInterface''' file calls the event functions in the [[CvEventManager|Event Manager]]. By editing this file, it becomes possible to create custom event managers. As with all interface files, it should not be imported, the function names should not be changed, and the functions in this file should not be placed into a class.

The Python files are written in the python programming language.  They can be edited in a text editor such as notepad or in a programming editor like Python's IDLE. 

==Functions==

Below is a list of all the functions in the file. Each function has a quick description attached to it. Note that there are comments strewn throughout some of these files, direct from the developers in order to aid the potential modders. These four functions are not in any class.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Function 
! style="background:#efefef;" | Parameters
! style="background:#efefef;" | Description
|-
!def getEventManager
|(No paramaters)
|Gets the event manager file (normally CvEventManager)
|-
!def onEvent
|argsList
|Called when a gave event happens and calls the event manager
|-
!def applyEvent
|argsList(context, playerID, netUserData, popupReturn)
|Applies events from the event manager
|-
!def beginEvent
|context, argsList=-1
|Begins an event in the event manager
|-
|}


==Example==

This example is a quick idea of what you can do in this file. While the four functions themselves should not be altered, you can add a custom event manager to the game by editing the top of the file, above the functions.

  import CvEventManager
  from CvPythonExtensions import *
  
  normalEventManager = CvEventManager.CvEventManager()

If you create and then import a "CvCustomEventManager" file and then make normalEventManager point to that instead, the game will not read CvEventManager as the event manager but instead your custom file, like so.

  import CvEventManager
  from CvPythonExtensions import *
  <font color="red">import CvCustomEventManager</font color>
  
  normalEventManager = <font color="red">CvCustomEventManager.CvCustomEventManager()</font color>

{{Civ4_Python_Files}}
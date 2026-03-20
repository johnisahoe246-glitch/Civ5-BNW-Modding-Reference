The '''CvDawnOfMan''' file is a python interface file that controls the appearance of the screen you get after first starting a game, called the "Dawn of Man" screen. It defines the popup screen and everything in it.

The Python files are written in the python programming language.  They can be edited in a text editor such as notepad or in a programming editor like Python's IDLE. 

==Functions==

Below is a list of all the functions in the file. Each function has a quick description attached to it. Note that there are comments strewn throughout some of these files, direct from the developers in order to aid the potential modders.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Function 
! style="background:#efefef;" | Parameters
! style="background:#efefef;" | Description
|-
!def _init_
|self, screenID
|Initializes variables, including screen dimensions
|-
!def interfaceScreen
|self
|Creates a popup to display the opening text
|-
!def handleInput
|self, inputClass
|Called when you get input like a button being clicked
|-
!def update
|self, fDelta
|Updates the screen (every frame?)
|-
!def onClose
|self
|Called when you close the screen
|-
!def calculateSizesAndPositions
|self
|Calculates size and position of screen
|}


==Example==

This example is a quick idea of what you can do with functions in this file. It adds your leaderhead art to the screen. 

 # Leaderhead graphic
 szLeaderPanel = "DawnOfManLeaderPanel"
 screen.addPanel( szLeaderPanel, "", "", true, false,
 	 self.X_LEADER_ICON - 3, self.Y_LEADER_ICON - 5, self.W_LEADER_ICON + 6, self.H_LEADER_ICON + 8, PanelStyles.PANEL_STYLE_DAWNTOP )
 screen.addLeaderheadGFC("LeaderHead", self.player.getLeaderType(), AttitudeTypes.ATTITUDE_PLEASED,
 	 self.X_LEADER_ICON + 5, self.Y_LEADER_ICON + 5, self.W_LEADER_ICON - 10, self.H_LEADER_ICON - 10, WidgetTypes.WIDGET_GENERAL, -1, -1)

{{Civ4_Python_Files}}
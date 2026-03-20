{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Container}} UIElement:LookUpControl<b>(</b>'''string''' arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">local unitPanel = ContextPtr:LookUpControl( "/InGame/WorldView/UnitPanel/Base" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">local infoCorner = ContextPtr:LookUpControl( "/InGame/WorldView/InfoCorner" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">ContextPtr:LookUpControl( "/InGame/WorldView/CityBannerManager" ):SetHide( not bCityBanners );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">ContextPtr:LookUpControl( "/InGame/WorldView/UnitFlagManager" ):SetHide( not bUnitFlags );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussLeader.lua}}
:<code>UI/InGame/LeaderHead/DiscussLeader.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0010}}<syntaxhighlight lang="lua">ContextPtr:LookUpControl( "../DiscussionOptions" ):SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ExitConfirm.lua}}
:<code>UI/FrontEnd/ExitConfirm.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">local inGame = ContextPtr:LookUpControl("/InGame");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0715}}<syntaxhighlight lang="lua">local contextID = ContextPtr:LookUpControl(".."):GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">local bIsModding = (ContextPtr:LookUpControl(".."):GetID() == "ModMultiplayerSelectScreen");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">bIsModding = (ContextPtr:LookUpControl("../.."):GetID() == "ModMultiplayerSelectScreen");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">m_pPlotHelpText = ContextPtr:LookUpControl( "/InGame/WorldView/PlotHelpText" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PreGameScreen.lua}}
:<code>UI/FrontEnd/PreGameScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">ContextPtr:LookUpControl( "../MainMenuScreenUI" ):SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectDifficulty.lua}}
:<code>UI/FrontEnd/GameSetup/SelectDifficulty.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">ContextPtr:LookUpControl( "../MainSelection" ):SetHide( false );</syntaxhighlight>
{{CodeLine5|0010}}<syntaxhighlight lang="lua">ContextPtr:LookUpControl( ".." ):SetHide( false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">g_isModding = (ContextPtr:LookUpControl(".."):GetID() == "ModdingGameSetupScreen") or (ContextPtr:LookUpControl("../../.."):GetID() == "ModMultiplayerSelectScreen");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">local g_SelectedContainer = ContextPtr:LookUpControl( "../SelectedUnitContainer" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1359}}<syntaxhighlight lang="lua">local EnemyUnitPanel = ContextPtr:LookUpControl( "/InGame/WorldView/EnemyUnitPanel" );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LookUpControl]]
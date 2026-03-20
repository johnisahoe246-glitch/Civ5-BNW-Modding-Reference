{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' UIElement:GetID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local m_bIsEndGame = (ContextPtr:GetID() == "EndGameDemographics");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local bIsModding = (ContextPtr:GetID() == "ModdingGameSetupScreen");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HallOfFame.lua}}
:<code>UI/InGame/Popups/HallOfFame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local m_bIsEndGame = (ContextPtr:GetID() == "EndGameHallOfFame");</syntaxhighlight>
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


{{PseudoH4|MultiplayerSelect.lua}}
:<code>UI/FrontEnd/Multiplayer/MultiplayerSelect.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0004}}<syntaxhighlight lang="lua">local bIsModding = (ContextPtr:GetID() == "ModMultiplayerSelectScreen");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">local bIsInGame = (ContextPtr:GetID() == "OptionsMenu_InGame");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">local bIsInGame = (ContextPtr:GetID() == "OptionsMenu_InGame"); --(UI.GetCurrentGameState() == GameStateTypes.CIV5_GS_MAINGAMEVIEW);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0149}}<syntaxhighlight lang="lua">g_bIsEndGame = (ContextPtr:GetID() == "EndGameReplay");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">g_isModding = (ContextPtr:LookUpControl(".."):GetID() == "ModdingGameSetupScreen") or (ContextPtr:LookUpControl("../../.."):GetID() == "ModMultiplayerSelectScreen");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetID]]
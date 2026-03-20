{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SelectionListGameNetMessage<b>(</b>{{Type5|GameMessageType}} message, '''int''' data2 = -1, {{Type5|BuildActionType}} data3 = -1, {{Type5|UnitID}} data4 = -1, '''int''' flags = 0, '''bool''' alt = false, '''bool''' shift = false<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|message:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|data2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|data3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|data4:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|flags:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alt:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shift:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ConfirmCommandPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmCommandPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(gameMessageDoCommand, action.CommandType, action.CommandData, -1, 0, bAlt);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ConfirmImprovementRebuildPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmImprovementRebuildPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(gameMessagePushMission, pAction.MissionType, pAction.MissionData, -1, 0, bAlt);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarRangeStrikePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarRangeStrikePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(messagePushMission, missionRangeAttack, iX, iY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MinorCivEnterTerritoryPopup.lua}}
:<code>UI/InGame/PopupsGeneric/MinorCivEnterTerritoryPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(messagePushMission, missionMoveTo, iX, iY, nil, false, bShift);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(GameMessageTypes.GAMEMESSAGE_PUSH_MISSION, eInterfaceModeMission, plotX, plotY, 0, false, bShift);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0446}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(GameMessageTypes.GAMEMESSAGE_PUSH_MISSION, MissionTypes.MISSION_RANGE_ATTACK, plotX, plotY, 0, false, bShift);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(GameMessageTypes.GAMEMESSAGE_PUSH_MISSION, MissionTypes.MISSION_EMBARK, plotX, plotY, 0, false, bShift);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0537}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(GameMessageTypes.GAMEMESSAGE_PUSH_MISSION, MissionTypes.MISSION_DISEMBARK, plotX, plotY, 0, false, bShift);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0635}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(GameMessageTypes.GAMEMESSAGE_PUSH_MISSION, iMission, plotX, plotY, 0, false, bShift);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(GameMessageTypes.GAMEMESSAGE_PUSH_MISSION, MissionTypes.MISSION_GARRISON, plotX, plotY, 0, false, bShift);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0660}}<syntaxhighlight lang="lua">Game.SelectionListGameNetMessage(GameMessageTypes.GAMEMESSAGE_DO_COMMAND, CommandTypes.COMMAND_CANCEL_ALL);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SelectionListGameNetMessage]]
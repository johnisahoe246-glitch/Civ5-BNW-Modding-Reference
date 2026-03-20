{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SelectedCitiesGameNetMessage<b>(</b>{{Type5|GameMessageType}} message, {{Type5|TaskType}} data2, '''int''' data3, {{Type5|BuildingType}} data4, '''bool''' option, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>


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
|valign="top" style="padding-right:6px;"|option:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alt:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shift:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ctrl:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1912}}<syntaxhighlight lang="lua">Game.SelectedCitiesGameNetMessage(GameMessageTypes.GAMEMESSAGE_POP_ORDER, num);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1931}}<syntaxhighlight lang="lua">Game.SelectedCitiesGameNetMessage(GameMessageTypes.GAMEMESSAGE_SWAP_ORDER, num);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1979}}<syntaxhighlight lang="lua">Game.SelectedCitiesGameNetMessage(GameMessageTypes.GAMEMESSAGE_DO_TASK, TaskTypes.TASK_NO_AUTO_ASSIGN_SPECIALISTS, -1, -1, bValue);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2035}}<syntaxhighlight lang="lua">Game.SelectedCitiesGameNetMessage(GameMessageTypes.GAMEMESSAGE_DO_TASK, TaskTypes.TASK_NO_AUTO_ASSIGN_SPECIALISTS, -1, -1, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2043}}<syntaxhighlight lang="lua">Game.SelectedCitiesGameNetMessage(GameMessageTypes.GAMEMESSAGE_DO_TASK, TaskTypes.TASK_ADD_SPECIALIST, iSpecialist, iBuilding);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2066}}<syntaxhighlight lang="lua">Game.SelectedCitiesGameNetMessage(GameMessageTypes.GAMEMESSAGE_DO_TASK, TaskTypes.TASK_REMOVE_SPECIALIST, iSpecialist, iBuilding);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0488}}<syntaxhighlight lang="lua">Game.SelectedCitiesGameNetMessage(GameMessageTypes.GAMEMESSAGE_DO_TASK, TaskTypes.TASK_RANGED_ATTACK, plotX, plotY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SelectedCitiesGameNetMessage]]
[[Category:Civ5 Cities API|SelectedCitiesGameNetMessage]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:AddFreeUnit<b>(</b>{{Type5|UnitType}} arg0, {{Type5|UnitAIType}} UNITAI_DEFENSE<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|UNITAI_DEFENSE:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">Players[0]:AddFreeUnit(70,5);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">Players[0]:AddFreeUnit(63,8);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">Players[0]:AddFreeUnit(66,6);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0303}}<syntaxhighlight lang="lua">pPlayer:AddFreeUnit (GameInfo.Units["UNIT_PIKEMAN"].ID, UNITAI_DEFENSE);</syntaxhighlight>
{{CodeLine5|0304}}<syntaxhighlight lang="lua">pPlayer:AddFreeUnit (GameInfo.Units["UNIT_CROSSBOWMAN"].ID, UNITAI_DEFENSE);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddFreeUnit]]
[[Category:Civ5 Units API|AddFreeUnit]]
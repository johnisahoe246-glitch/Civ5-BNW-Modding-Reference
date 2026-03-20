{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetSlotStatus<b>(</b>{{Type5|PlayerID}} i, {{Type5|SlotStatus}} arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0285}}<syntaxhighlight lang="lua">PreGame.SetSlotStatus(i, SlotStatus.SS_OPEN);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1157}}<syntaxhighlight lang="lua">PreGame.SetSlotStatus(i, SlotStatus.SS_COMPUTER);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">PreGame.SetSlotStatus(12, SlotStatus.SS_COMPUTER);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">PreGame.SetSlotStatus( playerID, SlotStatus.SS_COMPUTER );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">PreGame.SetSlotStatus( playerID, SlotStatus.SS_TAKEN );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1239}}<syntaxhighlight lang="lua">PreGame.SetSlotStatus( playerID, SlotStatus.SS_CLOSED );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">PreGame.SetSlotStatus(i, SlotStatus.SS_CLOSED);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetSlotStatus]]
[[Category:Civ5 Game Settings API|SetSlotStatus]]
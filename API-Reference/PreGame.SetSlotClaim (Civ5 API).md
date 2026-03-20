{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetSlotClaim<b>(</b>{{Type5|PlayerID}} player, {{Type5|SlotClaim}} arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1254}}<syntaxhighlight lang="lua">PreGame.SetSlotClaim( playerID, SlotClaim.SLOTCLAIM_RESERVED );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1256}}<syntaxhighlight lang="lua">PreGame.SetSlotClaim( playerID, SlotClaim.SLOTCLAIM_UNASSIGNED );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">PreGame.SetSlotClaim(i, SlotClaim.SLOTCLAIM_ASSIGNED);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetSlotClaim]]
[[Category:Civ5 Game Settings API|SetSlotClaim]]
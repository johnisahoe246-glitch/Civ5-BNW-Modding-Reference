{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetMinorCivNumActiveQuestsForPlayer<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0496}}<syntaxhighlight lang="lua">if( ( pOtherPlayer:GetMinorCivNumActiveQuestsForPlayer(g_iPlayer) == 0 and not pOtherPlayer:IsThreateningBarbariansEventActiveForPlayer(g_iPlayer) )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua (G&K)}}
:<code>DLC/Expansion/Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1127}}<syntaxhighlight lang="lua">if (pOtherPlayer:GetMinorCivNumActiveQuestsForPlayer(player:GetID()) >= 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMinorCivNumActiveQuestsForPlayer]]
[[Category:Civ5 Players API|GetMinorCivNumActiveQuestsForPlayer]]
[[Category:Civ5 City States API|GetMinorCivNumActiveQuestsForPlayer]]
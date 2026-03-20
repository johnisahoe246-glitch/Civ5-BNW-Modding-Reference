{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsDenouncingPlayer<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


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

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">elseif (pOtherPlayer:IsDenouncingPlayer(g_iPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">elseif (pOtherPlayer:IsDenouncingPlayer(iPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">elseif (Players[g_iAIPlayer]:IsDenouncingPlayer(iActivePlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">elseif (Players[g_iAIPlayer]:IsDenouncingPlayer(Game.GetActivePlayer())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0800}}<syntaxhighlight lang="lua">elseif (Players[iLeader]:IsDenouncingPlayer(iActivePlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsDenouncingPlayer]]
[[Category:Civ5 Players API|IsDenouncingPlayer]]
[[Category:Civ5 Diplomacy API|IsDenouncingPlayer]]
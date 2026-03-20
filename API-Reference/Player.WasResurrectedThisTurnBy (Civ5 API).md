{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:WasResurrectedThisTurnBy<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


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
{{CodeLine5|0309}}<syntaxhighlight lang="lua">elseif (pOtherPlayer:WasResurrectedThisTurnBy(g_iPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">elseif (pOtherPlayer:WasResurrectedThisTurnBy(iPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">elseif (Players[g_iAIPlayer]:WasResurrectedThisTurnBy(iActivePlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|WasResurrectedThisTurnBy]]
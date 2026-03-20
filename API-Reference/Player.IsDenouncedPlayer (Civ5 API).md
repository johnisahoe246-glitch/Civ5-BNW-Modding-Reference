{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsDenouncedPlayer<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|otherPlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">if (Players[g_iUs]:IsDenouncedPlayer(iOtherPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0221}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsDenouncedPlayer(iThirdPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">if(not activePlayer:IsDenouncedPlayer(iPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0813}}<syntaxhighlight lang="lua">if (pActivePlayer:IsDenouncedPlayer(iOtherPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0816}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsDenouncedPlayer(iActivePlayer)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsDenouncedPlayer]]
[[Category:Civ5 Players API|IsDenouncedPlayer]]
[[Category:Civ5 Diplomacy API|IsDenouncedPlayer]]
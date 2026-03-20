{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsFriendDenouncedUs<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsFriendDenouncedUs(g_iUs) or pOtherPlayer:IsFriendDeclaredWarOnUs(g_iUs)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0239}}<syntaxhighlight lang="lua">if (pThirdPlayer:IsFriendDenouncedUs(iOtherPlayer) or pThirdPlayer:IsFriendDeclaredWarOnUs(iOtherPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0801}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsFriendDenouncedUs(iActivePlayer)) then         -- Human was a friend and denounced us</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsFriendDenouncedUs]]
[[Category:Civ5 Diplomacy API|IsFriendDenouncedUs]]
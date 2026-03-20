{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsProtectingMinor<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


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

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0489}}<syntaxhighlight lang="lua">if (bWar or not bFriends or pActivePlayer:IsProtectingMinor(iPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0645}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsProtectingMinor(g_iMinorCivID)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsProtectingMinor(iMinor)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsProtectingMinor]]
[[Category:Civ5 Diplomacy API|IsProtectingMinor]]
[[Category:Civ5 City States API|IsProtectingMinor]]
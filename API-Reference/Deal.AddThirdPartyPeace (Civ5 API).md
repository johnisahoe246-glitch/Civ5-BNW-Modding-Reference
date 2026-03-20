{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:AddThirdPartyPeace<b>(</b>{{Type5|PlayerID}} who, {{Type5|TeamID}} otherPlayer, '''int''' arg2<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|who:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|otherPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2701}}<syntaxhighlight lang="lua">g_Deal:AddThirdPartyPeace( iWho, iOtherPlayer, GameDefines.PEACE_TREATY_LENGTH );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2958}}<syntaxhighlight lang="lua">g_Deal:AddThirdPartyPeace( iWho, iOtherTeam, GameDefines.PEACE_TREATY_LENGTH );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddThirdPartyPeace]]
[[Category:Civ5 Diplomacy API|AddThirdPartyPeace]]
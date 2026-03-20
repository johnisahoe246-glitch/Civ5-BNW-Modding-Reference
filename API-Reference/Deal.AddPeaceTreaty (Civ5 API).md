{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Deal:AddPeaceTreaty<b>(</b>{{Type5|PlayerID}} us, '''int''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">g_Deal:AddPeaceTreaty( g_iUs, GameDefines.PEACE_TREATY_LENGTH );</syntaxhighlight>
{{CodeLine5|0294}}<syntaxhighlight lang="lua">g_Deal:AddPeaceTreaty( g_iThem, GameDefines.PEACE_TREATY_LENGTH );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddPeaceTreaty]]
[[Category:Civ5 Diplomacy API|AddPeaceTreaty]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|PlayerID}} UI.HasMadeProposal<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|us:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">local iProposalTo = UI.HasMadeProposal( iUs );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">local iProposalTo = UI.HasMadeProposal( g_iUs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">elseif( UI.HasMadeProposal( g_iUs ) == g_iThem ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasMadeProposal]]
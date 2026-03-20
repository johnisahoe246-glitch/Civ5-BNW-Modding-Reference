{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:IsOpenBordersTradingAllowed<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (not owner:IsMinorCiv() and Teams[Game.GetActiveTeam()]:IsOpenBordersTradingAllowed()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1072}}<syntaxhighlight lang="lua">if (not g_pUsTeam:IsOpenBordersTradingAllowed() and not g_pThemTeam:IsOpenBordersTradingAllowed()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsOpenBordersTradingAllowed]]
[[Category:Civ5 Diplomacy API|IsOpenBordersTradingAllowed]]
[[Category:Civ5 Trade API|IsOpenBordersTradingAllowed]]
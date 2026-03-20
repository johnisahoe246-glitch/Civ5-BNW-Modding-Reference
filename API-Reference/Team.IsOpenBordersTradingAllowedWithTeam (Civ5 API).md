{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Team:IsOpenBordersTradingAllowedWithTeam<b>(</b>{{Type5|TeamID}} arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DeclareWarMovePopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">if (not owner:IsMinorCiv() and Teams[Game.GetActiveTeam()]:IsOpenBordersTradingAllowedWithTeam(plot:GetTeam())) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsOpenBordersTradingAllowedWithTeam]]
[[Category:Civ5 Diplomacy API|IsOpenBordersTradingAllowedWithTeam]]
[[Category:Civ5 Trade API|IsOpenBordersTradingAllowedWithTeam]]
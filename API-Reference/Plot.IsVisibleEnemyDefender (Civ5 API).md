{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsVisibleEnemyDefender<b>(</b>{{Type5|Unit}} unit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">if (plot:IsVisible(player:GetTeam(), false) and (plot:IsVisibleEnemyDefender(pUnit) or plot:IsEnemyCity(pUnit))) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsVisibleEnemyDefender]]
[[Category:Civ5 Fog API|IsVisibleEnemyDefender]]
[[Category:Civ5 Combat API|IsVisibleEnemyDefender]]
[[Category:Civ5 Diplomacy API|IsVisibleEnemyDefender]]
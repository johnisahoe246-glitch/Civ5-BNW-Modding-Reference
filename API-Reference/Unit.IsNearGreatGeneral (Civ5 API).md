{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:IsNearGreatGeneral<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0771}}<syntaxhighlight lang="lua">if (pMyUnit:IsNearGreatGeneral()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1157}}<syntaxhighlight lang="lua">if (pTheirUnit:IsNearGreatGeneral()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1512}}<syntaxhighlight lang="lua">if (theirUnit:IsNearGreatGeneral()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsNearGreatGeneral]]
[[Category:Civ5 Great People API|IsNearGreatGeneral]]
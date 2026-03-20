{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:OpenDefenseModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1300}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:OpenDefenseModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1572}}<syntaxhighlight lang="lua">iModifier = theirUnit:OpenDefenseModifier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OpenDefenseModifier]]
[[Category:Civ5 Combat API|OpenDefenseModifier]]
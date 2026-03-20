{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsGoldenAge<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1066}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pMyPlayer:IsGoldenAge()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1387}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and pTheirPlayer:IsGoldenAge()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1648}}<syntaxhighlight lang="lua">if (iModifier ~= 0 and theirPlayer:IsGoldenAge()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsGoldenAge]]
[[Category:Civ5 Golden Age API|IsGoldenAge]]
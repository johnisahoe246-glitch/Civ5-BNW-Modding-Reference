{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetFriendlyLandsModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0827}}<syntaxhighlight lang="lua">iModifier = pMyUnit:GetFriendlyLandsModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1203}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:GetFriendlyLandsModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1531}}<syntaxhighlight lang="lua">iModifier = theirUnit:GetFriendlyLandsModifier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFriendlyLandsModifier]]
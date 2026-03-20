{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:CapitalDefenseModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0923}}<syntaxhighlight lang="lua">iModifier = pMyUnit:CapitalDefenseModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1472}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:CapitalDefenseModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1814}}<syntaxhighlight lang="lua">iModifier = theirUnit:CapitalDefenseModifier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CapitalDefenseModifier]]
[[Category:Civ5 Cities API|CapitalDefenseModifier]]
[[Category:Civ5 Combat API|CapitalDefenseModifier]]
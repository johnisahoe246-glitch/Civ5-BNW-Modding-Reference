{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:CapitalDefenseFalloff<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0932}}<syntaxhighlight lang="lua">iModifier = iModifier + (plotDistance * pMyUnit:CapitalDefenseFalloff());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1481}}<syntaxhighlight lang="lua">iModifier = iModifier + (plotDistance * pTheirUnit:CapitalDefenseFalloff());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1822}}<syntaxhighlight lang="lua">iModifier = iModifier + (plotDistance * theirUnit:CapitalDefenseFalloff());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CapitalDefenseFalloff]]
[[Category:Civ5 Cities API|CapitalDefenseFalloff]]
[[Category:Civ5 Combat API|CapitalDefenseFalloff]]
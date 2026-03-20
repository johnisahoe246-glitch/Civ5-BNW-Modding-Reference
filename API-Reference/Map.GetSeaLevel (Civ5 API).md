{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Map.GetSeaLevel<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ContinentsWorld.lua}}
:<code>Gameplay/Lua/ContinentsWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">local sea_level = GameInfo.SeaLevels[Map.GetSeaLevel()];</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSeaLevel]]
[[Category:Civ5 Terrain API|GetSeaLevel]]
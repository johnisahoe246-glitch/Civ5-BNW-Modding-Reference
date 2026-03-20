{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|FractalWorld}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' FractalWorld:GenerateCenterRift<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0559}}<syntaxhighlight lang="lua">self:GenerateCenterRift()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">SetPlotTypes(self.plotTypes);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0756}}<syntaxhighlight lang="lua">self:GenerateCenterRift()</syntaxhighlight>
{{CodeLine5|0757}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenerateCenterRift]]
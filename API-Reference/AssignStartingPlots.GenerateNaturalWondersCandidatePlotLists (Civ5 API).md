{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>table('''int''' => '''int''') AssignStartingPlots:GenerateNaturalWondersCandidatePlotLists<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5993}}<syntaxhighlight lang="lua">local NW_eligibility_order = self:GenerateNaturalWondersCandidatePlotLists()</syntaxhighlight>
{{CodeLine5|5994}}<syntaxhighlight lang="lua">local iNumNWCandidates = table.maxn(NW_eligibility_order);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenerateNaturalWondersCandidatePlotLists]]
[[Category:Civ5 Features & Natural wonders API|GenerateNaturalWondersCandidatePlotLists]]
[[Category:Civ5 Buildings API|GenerateNaturalWondersCandidatePlotLists]]
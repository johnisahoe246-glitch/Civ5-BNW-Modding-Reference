{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:__InitLuxuryWeights<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0504}}<syntaxhighlight lang="lua">findStarts:__InitLuxuryWeights()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0506}}<syntaxhighlight lang="lua">-- Entry point for easy overrides, for instance if only a couple things need to change.</syntaxhighlight>
{{CodeLine5|0507}}<syntaxhighlight lang="lua">findStarts:__CustomInit()</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|__InitLuxuryWeights]]
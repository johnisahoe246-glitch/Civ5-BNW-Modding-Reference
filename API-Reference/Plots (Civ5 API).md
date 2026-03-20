{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapGenerator.lua")</code>
}}


=Usage=
<code>iterator() Plots<b>(</b>('''void''' func<b>(</b>table('''int''' => '''int''') t<b>)</b>) sort = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|sort:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0842}}<syntaxhighlight lang="lua">for i, plot in Plots() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0694}}<syntaxhighlight lang="lua">for index, plot in Plots(Shuffle) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">for index, plot in Plots() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">for i, plot in Plots(Shuffle) do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Plots]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Plot:IsImpassable<b>(</b><b>)</b></code>


'''Returned Value'''
:This will not always return false for Mountain plots.

=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0617}}<syntaxhighlight lang="lua">if (plot:IsImpassable()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsImpassable]]
[[Category:Civ5 Movement API|IsImpassable]]
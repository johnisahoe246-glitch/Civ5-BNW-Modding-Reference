{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>'''void''' PrintContentsOfTable<b>(</b>table('''int''' => '''int''') incoming_table<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|incoming_table:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1698}}<syntaxhighlight lang="lua">PrintContentsOfTable(numberOfCivsPerArea)</syntaxhighlight>
{{CodeLine5|1699}}<syntaxhighlight lang="lua">print("--- End of Civs per Landmass readout ***"); print("-"); print("-");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PrintContentsOfTable]]
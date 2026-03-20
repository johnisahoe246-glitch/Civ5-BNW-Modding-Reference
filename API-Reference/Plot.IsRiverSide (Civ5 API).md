{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Plot:IsRiverSide<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0822}}<syntaxhighlight lang="lua">if plot:IsRiverSide() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2353}}<syntaxhighlight lang="lua">if searchPlot:IsRiverSide() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3569}}<syntaxhighlight lang="lua">elseif plot:IsRiverSide() then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsRiverSide]]
[[Category:Civ5 Rivers API|IsRiverSide]]
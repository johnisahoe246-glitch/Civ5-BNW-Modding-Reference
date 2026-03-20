{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>table('''int''' => '''int''') ObtainLandmassBoundaries<b>(</b>{{Type5|AreaID}} areaID<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|areaID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1478}}<syntaxhighlight lang="lua">local landmass_data = ObtainLandmassBoundaries(iAreaID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1707}}<syntaxhighlight lang="lua">local landmass_data = ObtainLandmassBoundaries(currentLandmassID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ObtainLandmassBoundaries]]
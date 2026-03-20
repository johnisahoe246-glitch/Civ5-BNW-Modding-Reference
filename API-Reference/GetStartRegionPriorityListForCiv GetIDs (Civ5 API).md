{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>table('''int''' => '''int''') GetStartRegionPriorityListForCiv_GetIDs<b>(</b>'''string''' civType<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|civType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4658}}<syntaxhighlight lang="lua">local table_of_this_civs_priority_needs = GetStartRegionPriorityListForCiv_GetIDs(civType)</syntaxhighlight>
{{CodeLine5|4659}}<syntaxhighlight lang="lua">iNumPriorityCivs = iNumPriorityCivs + 1;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetStartRegionPriorityListForCiv_GetIDs]]
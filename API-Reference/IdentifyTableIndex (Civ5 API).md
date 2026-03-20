{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("MapmakerUtilities.lua")</code>
}}


=Usage=
<code>'''bool''', '''int''', table('''int''' => '''int''') IdentifyTableIndex<b>(</b>table('''int''' => {{Type5|PlayerID}}) incoming_table, {{Type5|PlayerID}} value<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|incoming_table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|value:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4742}}<syntaxhighlight lang="lua">local a, b, c = IdentifyTableIndex(civs_needing_coastal_start, playerNum)</syntaxhighlight>
{{CodeLine5|4743}}<syntaxhighlight lang="lua">if a then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4746}}<syntaxhighlight lang="lua">local a, b, c = IdentifyTableIndex(regions_still_available, choose_this_region)</syntaxhighlight>
{{CodeLine5|4747}}<syntaxhighlight lang="lua">if a then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5902}}<syntaxhighlight lang="lua">local bFoundValue, iNumTimesFoundValue, table_of_indices = IdentifyTableIndex(NW_remaining_to_sort_by_occurrence, possible_selection)</syntaxhighlight>
{{CodeLine5|5903}}<syntaxhighlight lang="lua">if bFoundValue then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IdentifyTableIndex]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:ChopIntoTwoRegions<b>(</b>'''unknown''' fertility_table, '''table''' rectangle_data_table, '''bool''' taller, '''float''' chopPercent<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fertility_table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|rectangle_data_table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|taller:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|chopPercent:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1175}}<syntaxhighlight lang="lua">local results = self:ChopIntoTwoRegions(fertility_table, rectangle_data_table, bTaller, chopPercent);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1187}}<syntaxhighlight lang="lua">local results = self:ChopIntoTwoRegions(fertility_table, rectangle_data_table, bTaller, 49.5); -- Undershoot by design, to compensate for inevitable overshoot. Gets the actual result closer to target.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1223}}<syntaxhighlight lang="lua">local initial_results = self:ChopIntoTwoRegions(fertility_table, rectangle_data_table, bTaller, 33); -- Undershoot by a bit, tends to make the actual result closer to accurate.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1256}}<syntaxhighlight lang="lua">local interim_results = self:ChopIntoTwoRegions(second_section_fertility_table, second_section_data_table, bTallerForRemainder, 48.5); -- Undershoot just a little.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0949}}<syntaxhighlight lang="lua">local results = self:ChopIntoTwoRegions(fertility_table, rectangle_data_table, bTaller, 38.5); -- CUSTOM, give Celtic region less land!</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChopIntoTwoRegions]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:DivideIntoRegions<b>(</b>'''int''' numDivisions, '''unknown''' fertility_table, '''table''' rectangle_data_table<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|numDivisions:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|fertility_table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|rectangle_data_table:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 47 are listed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1181}}<syntaxhighlight lang="lua">self:DivideIntoRegions(firstSubdivisions, first_section_fertility_table, first_section_data_table)</syntaxhighlight>
{{CodeLine5|1182}}<syntaxhighlight lang="lua">self:DivideIntoRegions(laterSubdivisions, second_section_fertility_table, second_section_data_table)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1184}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1193}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iSubdivisions, first_section_fertility_table, first_section_data_table)</syntaxhighlight>
{{CodeLine5|1194}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iSubdivisions, second_section_fertility_table, second_section_data_table)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1196}}<syntaxhighlight lang="lua">elseif (iNumDivides == 3) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1207}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iSubdivisions, second_section_fertility_table, second_section_data_table)</syntaxhighlight>
{{CodeLine5|1208}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iSubdivisions, third_section_fertility_table, third_section_data_table)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1210}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1504}}<syntaxhighlight lang="lua">self:DivideIntoRegions(self.iNumCivs, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1505}}<syntaxhighlight lang="lua">-- The regions have been defined.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1507}}<syntaxhighlight lang="lua">elseif self.method == 3 or self.method == 4 then -- Rectangular</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1525}}<syntaxhighlight lang="lua">self:DivideIntoRegions(self.iNumCivs, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1526}}<syntaxhighlight lang="lua">-- The regions have been defined.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1528}}<syntaxhighlight lang="lua">else -- Continental.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1735}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iNumCivsOnThisLandmass, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1736}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0865}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0866}}<syntaxhighlight lang="lua">iNumCivsRemaining = iNumCivsRemaining - 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0887}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iNumCivsRemaining, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0888}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0956}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iSubdivisions, second_section_fertility_table, second_section_data_table)</syntaxhighlight>
{{CodeLine5|0957}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0997}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0998}}<syntaxhighlight lang="lua">--print("- Morocco and Tunisia defined as Region 3.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1000}}<syntaxhighlight lang="lua">-- Egypt and Judea.</syntaxhighlight>
{{CodeLine5|1001}}<syntaxhighlight lang="lua">self.inhabited_WestX = 56;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1009}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1010}}<syntaxhighlight lang="lua">--print("- Egypt and Judea defined as Region 4.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1012}}<syntaxhighlight lang="lua">-- Turkey.</syntaxhighlight>
{{CodeLine5|1013}}<syntaxhighlight lang="lua">self.inhabited_WestX = 60;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1021}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1022}}<syntaxhighlight lang="lua">--print("- Turkey defined as Region 5.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1024}}<syntaxhighlight lang="lua">-- Balkans.</syntaxhighlight>
{{CodeLine5|1025}}<syntaxhighlight lang="lua">self.inhabited_WestX = 42;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1033}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1034}}<syntaxhighlight lang="lua">--print("- Balkans defined as Region 6.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1036}}<syntaxhighlight lang="lua">-- Spain.</syntaxhighlight>
{{CodeLine5|1037}}<syntaxhighlight lang="lua">self.inhabited_WestX = 6;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1045}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1046}}<syntaxhighlight lang="lua">--print("- Spain defined as Region 7.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1049}}<syntaxhighlight lang="lua">self.inhabited_WestX = 6;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1057}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1058}}<syntaxhighlight lang="lua">--print("- France defined as Region 8.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1060}}<syntaxhighlight lang="lua">-- Netherlands.</syntaxhighlight>
{{CodeLine5|1061}}<syntaxhighlight lang="lua">self.inhabited_WestX = 19;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1069}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1070}}<syntaxhighlight lang="lua">--print("- Netherlands defined as Region 9.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1072}}<syntaxhighlight lang="lua">-- Central Europe.</syntaxhighlight>
{{CodeLine5|1073}}<syntaxhighlight lang="lua">self.inhabited_WestX = 35;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1081}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1082}}<syntaxhighlight lang="lua">--print("- Central Europe defined as Region 10.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1084}}<syntaxhighlight lang="lua">-- Scandinavia.</syntaxhighlight>
{{CodeLine5|1085}}<syntaxhighlight lang="lua">self.inhabited_WestX = 23;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1093}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1094}}<syntaxhighlight lang="lua">--print("- Scandinavia defined as Region 11.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1096}}<syntaxhighlight lang="lua">-- Russia.</syntaxhighlight>
{{CodeLine5|1097}}<syntaxhighlight lang="lua">self.inhabited_WestX = 51;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1105}}<syntaxhighlight lang="lua">self:DivideIntoRegions(1, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|1106}}<syntaxhighlight lang="lua">--print("- Russia defined as Region 12.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1108}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0967}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iNumCivsInWest, fert_table, rect_table)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0969}}<syntaxhighlight lang="lua">-- Process the team in the east.</syntaxhighlight>
{{CodeLine5|0970}}<syntaxhighlight lang="lua">self.inhabited_WestX = math.floor(iW / 2) + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0982}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iNumCivsInEast, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0983}}<syntaxhighlight lang="lua">-- The regions have been defined.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0985}}<syntaxhighlight lang="lua">-- If number of teams is any number other than two, use standard division.</syntaxhighlight>
{{CodeLine5|0986}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|North_vs_South.lua}}
:<code>Maps/North_vs_South.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iNumCivsInSouth, fert_table, rect_table)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0520}}<syntaxhighlight lang="lua">-- Process the team in the north.</syntaxhighlight>
{{CodeLine5|0521}}<syntaxhighlight lang="lua">self.inhabited_WestX = 0;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0533}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iNumCivsInNorth, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0534}}<syntaxhighlight lang="lua">-- The regions have been defined.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0536}}<syntaxhighlight lang="lua">-- If number of teams is any number other than two, use standard One Landmass division.</syntaxhighlight>
{{CodeLine5|0537}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0560}}<syntaxhighlight lang="lua">self:DivideIntoRegions(self.iNumCivs, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0561}}<syntaxhighlight lang="lua">-- The regions have been defined.</syntaxhighlight>
{{CodeLine5|0562}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|West_vs_East.lua}}
:<code>Maps/West_vs_East.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">self:DivideIntoRegions(iNumCivsInEast, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0356}}<syntaxhighlight lang="lua">-- The regions have been defined.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">-- If number of teams is any number other than two, use standard One Landmass division.</syntaxhighlight>
{{CodeLine5|0359}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DivideIntoRegions]]
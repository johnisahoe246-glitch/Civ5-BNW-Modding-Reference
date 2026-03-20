{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''', '''int''', '''int''', '''int''' AssignStartingPlots:CustomOverride<b>(</b>{{Type5|ResourceType}} resource_<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource_:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1497}}<syntaxhighlight lang="lua">self:CustomOverride()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1499}}<syntaxhighlight lang="lua">--[[ Printout is for debugging only. Deactivate otherwise.</syntaxhighlight>
{{CodeLine5|1500}}<syntaxhighlight lang="lua">local tempRegionData = self.regionData;</syntaxhighlight>
{{CodeLine5|1501}}<syntaxhighlight lang="lua">for i, data in ipairs(tempRegionData) do</syntaxhighlight>
{{CodeLine5|1502}}<syntaxhighlight lang="lua">   print("-");</syntaxhighlight>
{{CodeLine5|1503}}<syntaxhighlight lang="lua">   print("Data for Start Region #", i);</syntaxhighlight>
{{CodeLine5|1504}}<syntaxhighlight lang="lua">   print("WestX:  ", data[1]);</syntaxhighlight>
{{CodeLine5|1505}}<syntaxhighlight lang="lua">   print("SouthY: ", data[2]);</syntaxhighlight>
{{CodeLine5|1506}}<syntaxhighlight lang="lua">   print("Width:  ", data[3]);</syntaxhighlight>
{{CodeLine5|1507}}<syntaxhighlight lang="lua">   print("Height: ", data[4]);</syntaxhighlight>
{{CodeLine5|1508}}<syntaxhighlight lang="lua">   print("AreaID: ", data[5]);</syntaxhighlight>
{{CodeLine5|1509}}<syntaxhighlight lang="lua">   print("Fertility:", data[6]);</syntaxhighlight>
{{CodeLine5|1510}}<syntaxhighlight lang="lua">   print("Plots:  ", data[7]);</syntaxhighlight>
{{CodeLine5|1511}}<syntaxhighlight lang="lua">   print("Fert/Plot:", data[8]);</syntaxhighlight>
{{CodeLine5|1512}}<syntaxhighlight lang="lua">   print("-");</syntaxhighlight>
{{CodeLine5|1513}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|1514}}<syntaxhighlight lang="lua">   ]]--</syntaxhighlight>
{{CodeLine5|1515}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1745}}<syntaxhighlight lang="lua">self:CustomOverride()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1747}}<syntaxhighlight lang="lua">-- Printout is for debugging only. Deactivate otherwise.</syntaxhighlight>
{{CodeLine5|1748}}<syntaxhighlight lang="lua">local tempRegionData = self.regionData;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1176}}<syntaxhighlight lang="lua">primary, secondary, tertiary, quaternary = self:CustomOverride(res_ID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CustomOverride]]
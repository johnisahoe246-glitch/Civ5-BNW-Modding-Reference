{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''', '''int''', '''int''' AssignStartingPlots:MeasureStartPlacementFertilityInRectangle<b>(</b>'''int''' westX, '''int''' southY, '''int''' width, '''int''' height<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|westX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|southY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|width:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|height:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1519}}<syntaxhighlight lang="lua">local fert_table, fertCount, plotCount = self:MeasureStartPlacementFertilityInRectangle(self.inhabited_WestX,</syntaxhighlight>
{{CodeLine5|1520}}<syntaxhighlight lang="lua">self.inhabited_SouthY, self.inhabited_Width, self.inhabited_Height)</syntaxhighlight>
{{CodeLine5|1521}}<syntaxhighlight lang="lua">-- Assemble the Rectangle data table:</syntaxhighlight>
{{CodeLine5|1522}}<syntaxhighlight lang="lua">local rect_table = {self.inhabited_WestX, self.inhabited_SouthY, self.inhabited_Width,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0861}}<syntaxhighlight lang="lua">local fert_table, fertCount, plotCount = self:MeasureStartPlacementFertilityInRectangle(self.inhabited_WestX,</syntaxhighlight>
{{CodeLine5|0862}}<syntaxhighlight lang="lua">self.inhabited_SouthY, self.inhabited_Width, self.inhabited_Height)</syntaxhighlight>
{{CodeLine5|0863}}<syntaxhighlight lang="lua">local rect_table = {self.inhabited_WestX, self.inhabited_SouthY, self.inhabited_Width,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">local fert_table, fertCount, plotCount = self:MeasureStartPlacementFertilityInRectangle(iWestX, iSouthY, iWidth, iHeight)</syntaxhighlight>
{{CodeLine5|0592}}<syntaxhighlight lang="lua">local fAverageFertility = fertCount / plotCount;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MeasureStartPlacementFertilityInRectangle]]
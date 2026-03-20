{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''', {{Type5|AreaID}}, {{Type5|AreaID}} AssignStartingPlots:MeasureStartPlacementFertilityOfLandmass<b>(</b>{{Type5|AreaID}} areaID, {{Type5|AreaID}} westX, '''int''' eastX, {{Type5|AreaID}} southY, '''int''' northY, '''bool''' wrapsX, '''bool''' wrapsY<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|areaID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|westX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|eastX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|southY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|northY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|wrapsX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|wrapsY:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1491}}<syntaxhighlight lang="lua">local fert_table, fertCount, plotCount = self:MeasureStartPlacementFertilityOfLandmass(iAreaID,</syntaxhighlight>
{{CodeLine5|1492}}<syntaxhighlight lang="lua">iWestX, iEastX, iSouthY, iNorthY, wrapsX, wrapsY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1719}}<syntaxhighlight lang="lua">local fert_table, fertCount, plotCount = self:MeasureStartPlacementFertilityOfLandmass(currentLandmassID,</syntaxhighlight>
{{CodeLine5|1720}}<syntaxhighlight lang="lua">iWestX, iEastX, iSouthY, iNorthY, wrapsX, wrapsY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MeasureStartPlacementFertilityOfLandmass]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>table('''int''' => '''int'''), '''int''', '''int''', '''int''', '''int''' AssignStartingPlots:RemoveDeadRows<b>(</b>table('''int''' => '''int''') fertility_table, '''int''' westX, '''int''' southY, '''int''' width, '''int''' height<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fertility_table:
|valign="top"| ''No description available.''
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
{{CodeLine5|1428}}<syntaxhighlight lang="lua">FRFertT, FRWX, FRSY, FRWid, FRHei = self:RemoveDeadRows(region_one_fertility,</syntaxhighlight>
{{CodeLine5|1429}}<syntaxhighlight lang="lua">firstRegionWestX, firstRegionSouthY, firstRegionWidth, firstRegionHeight);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1433}}<syntaxhighlight lang="lua">SRFertT, SRWX, SRSY, SRWid, SRHei = self:RemoveDeadRows(region_two_fertility,</syntaxhighlight>
{{CodeLine5|1434}}<syntaxhighlight lang="lua">secondRegionWestX, secondRegionSouthY, secondRegionWidth, secondRegionHeight);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RemoveDeadRows]]
[[Category:Civ5 Combat API|RemoveDeadRows]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Plot}} Map.PlotXYWithRangeCheck<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset, '''int''' maxRange<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|xOffset:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|yOffset:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|maxRange:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0456}}<syntaxhighlight lang="lua">local evalPlot = Map.PlotXYWithRangeCheck(unitX, unitY, iX, iY, iRange);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0683}}<syntaxhighlight lang="lua">local pPlot = Map.PlotXYWithRangeCheck(iCityStateX, iCityStateY, iX, iY, iRange);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0639}}<syntaxhighlight lang="lua">local otherPlot = Map.PlotXYWithRangeCheck(plotX, plotY, dx, dy, uniqueRange);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0649}}<syntaxhighlight lang="lua">local otherPlot = Map.PlotXYWithRangeCheck(plotX, plotY, dx, dy, 4);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">local otherPlot   = Map.PlotXYWithRangeCheck(plot:GetX(), plot:GetY(), dx, dy, groupRange);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlotXYWithRangeCheck]]
[[Category:Civ5 Combat API|PlotXYWithRangeCheck]]
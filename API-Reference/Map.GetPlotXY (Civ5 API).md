{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Plot}} Map.GetPlotXY<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset<b>)</b></code>


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
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0298}}<syntaxhighlight lang="lua">local pTargetPlot = Map.GetPlotXY(thisX, thisY, iDX, iDY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">local pTargetPlot = Map.GetPlotXY(iPlotX, iPlotY, iDX, iDY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1437}}<syntaxhighlight lang="lua">local pTargetPlot = Map.GetPlotXY(iX, iY, iDX, iDY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">local otherPlot   = Map.GetPlotXY(plotX, plotY, dx, dy);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlotXY]]
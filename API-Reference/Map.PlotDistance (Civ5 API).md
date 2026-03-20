{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Map.PlotDistance<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset<b>)</b></code>


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
{{CodeLine5|0307}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(thisX, thisY, plotX, plotY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0931}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), pMyUnit:GetX(), pMyUnit:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1480}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), pTheirUnit:GetX(), pTheirUnit:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1821}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), theirUnit:GetX(), theirUnit:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(iPlotX, iPlotY, plotX, plotY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0556}}<syntaxhighlight lang="lua">iDistance = Map.PlotDistance(1, iY, pUnit:GetX(), pUnit:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">if (Map.PlotDistance(pCity:GetX(), pCity:GetY(), iLondonX, iLondonY) < 8) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1587}}<syntaxhighlight lang="lua">if (Map.PlotDistance(pReformerCity:GetX(), pReformerCity:GetY(), pCity:GetX(), pCity:GetY()) <= 10) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1560}}<syntaxhighlight lang="lua">if (Map.PlotDistance(pFirstUnitPlot:GetX(), pFirstUnitPlot:GetY(), pSecondUnitPlot:GetX(), pSecondUnitPlot:GetY()) <= iMovesLeft ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">if (Map.PlotDistance(plotX, plotY, otherPlot:GetX(), otherPlot:GetY()) <= uniqueRange) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlotDistance]]
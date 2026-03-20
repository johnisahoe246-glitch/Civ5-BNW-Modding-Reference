{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered every time the population of a city changes. The triggering city need not belong to the active (human) player, although the city needs to have been discovered by that player. Cities that the active player has no knowledge of will not trigger this event.


=Usage=
<code>'''void''' Events.SerialEventCityPopulationChanged<b>(</b>'''float''' hexX, '''int''' hexY, '''int''' newPop, '''int''' unknown<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventCityPopulationChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventCityPopulationChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''Hex x-coordinate of the city whose population changed which can be converted to map grid coordinates with the {{Type5|ToGridFromHex}} function (see example)''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''Hex y-coordinate of the city whose population changed which can be converted to map grid coordinates with the {{Type5|ToGridFromHex}} function (see example)''
|-
|valign="top" style="padding-right:6px;"|newPop:
|valign="top"| ''the new population of the city whose population changed''
|-
|valign="top" style="padding-right:6px;"|unknown:
|valign="top"| ''unsure what the meaning of this argument is, although it would always seem to be half of iNewPop, rounded up; possibly related to city graphics''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
function onCityPopulationChanged(iHexX, iHexY, iPopulation, iUnknown )
local pPlot = Map.GetPlot(ToGridFromHex(iHexX, iHexY))
local pCity = pPlot:GetPlotCity()
local iOwner = pCity:GetOwner()
print(string.format("%s (owned by %s) has grown to size %d", pCity:GetName(), Players[iOwner]:GetName(), iPopulation))
end
Events.SerialEventCityPopulationChanged.Add(onCityPopulationChanged)</syntaxhighlight>


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">Events.SerialEventCityPopulationChanged( g_iHexX, g_iHexY, g_iPopulation, iCitySize );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventCityPopulationChanged]]
[[Category:Civ5 Cities API|SerialEventCityPopulationChanged]]
[[Category:Civ5 Food & Population API|SerialEventCityPopulationChanged]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered whenever a route is built (triggers on railroads despite the name). The tile must have been discovered by the active player but doesn't have to be visible. This also triggers when a new city is founded, which immediately builds a road and railroad on the spot.


=Usage=
<code>'''void''' Events.SerialEventRoadCreated<b>(</b>'''int''' hexX, '''int''' hexY, {{Type5|PlayerID}} player, '''int''' routeType<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventRoadCreated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventRoadCreated(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''Hex x-coordinate of the tile the road was built on which can be converted to map grid coordinates with the {{Type5|ToGridFromHex}} function (see example)''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''Hex y-coordinate of the tile the road was built on which can be converted to map grid coordinates with the {{Type5|ToGridFromHex}} function (see example)''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''the ID of the player who built the road''
|-
|valign="top" style="padding-right:6px;"|routeType:
|valign="top"| ''the ID of the route type that was built''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
function onRoadCreated(iHexX, iHexY, iPlayerID, iRouteType)
local pPlot = Map.GetPlot(ToGridFromHex(iHexX, iHexY))
local plotOwner = pPlot:GetOwner() > -1 and Players[pPlot:GetOwner()]:GetName() or "nobody"
print(string.format("Route of type %d built on tile %d, %d by player %d. Plot owned by %s", iRouteType, pPlot:GetX(), pPlot:GetY(), iPlayerID, plotOwner))
end
Events.SerialEventRoadCreated.Add(onRoadCreated)</syntaxhighlight>


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0428}}<syntaxhighlight lang="lua">Events.SerialEventRoadCreated( g_iHexX, g_iHexY, g_iCurrPlayer, 0 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventRoadCreated]]
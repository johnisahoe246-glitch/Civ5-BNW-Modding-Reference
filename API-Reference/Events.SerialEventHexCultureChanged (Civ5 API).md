{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered every time a hex changes ownership anywhere on the map.


=Usage=
<code>'''void''' Events.SerialEventHexCultureChanged<b>(</b>'''int''' hexX, '''int''' hexY, {{Type5|PlayerID}} player, '''bool''' unknown<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''Hex x-coordinate of the tile whose ownership has changed. This can be converted to map grid (plot) coordinates with the {{Type5|ToGridFromHex}} function (see example)''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''Hex y-coordinate of the tile whose ownership has changed. This can be converted to map grid (plot) coordinates with the {{Type5|ToGridFromHex}} function (see example)''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''The ID of the new owner (key to the Players table)''
|-
|valign="top" style="padding-right:6px;"|unknown:
|valign="top"| ''Seems to be always false''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
function onHexCultureChanged(iHexX, iHexY, iPlayerID, bUnknown)
print(string.format("New hex claimed at coordinates: %d, %d for player: %d", iHexX, iHexY, iPlayerID))
end
Events.SerialEventHexCultureChanged.Add(onHexCultureChanged)</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventHexCultureChanged]]
[[Category:Civ5 Culture API|SerialEventHexCultureChanged]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


Like SerialEventImprovementCreated, this event is triggered whenever an improvement appears on a player's map, as a result of an improvement being created on a tile already been discovered by the active player, or a tile being discovered that already hosts an improvement. Barbarian camps and ancient ruins count as improvements, as listed on the Improvement table. A completed improvement replacing an improvement in progress will not trigger this event.


=Usage=
<code>'''void''' Events.SerialEventImprovementDestroyed<b>(</b>'''int''' hexX, '''int''' hexY, '''int''' continent1, '''int''' continent2<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''Hex y-coordinate of the tile the road was built on which can be converted to map grid coordinates with the {{Type5|ToGridFromHex}} function (see example)''
|-
|valign="top" style="padding-right:6px;"|continent1:
|valign="top"| ''These values appear to always be the same and also seem to refer to the continent on which the improvement was destroyed. Different land masses will have different numbers corresponding to their graphic set, and oceans will be marked as 0.''
|-
|valign="top" style="padding-right:6px;"|continent2:
|valign="top"| ''No description available.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
function onImprovementDestroyed(iHexX, iHexY, iContinent1, iContinent2)
local pPlot = Map.GetPlot(ToGridFromHex(iHexX, iHexY))
local plotOwner = pPlot:GetOwner() > -1 and Players[pPlot:GetOwner()]:GetName() or "nobody"
print(string.format("Improvement destroyed on tile %d, %d by player %d. Plot owned by %s", pPlot:GetX(), pPlot:GetY(), iPlayerID, plotOwner))
end
Events.SerialEventImprovementDestroyed.Add(onImprovementDestroyed)</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventImprovementDestroyed]]
[[Category:Civ5 Improvements API|SerialEventImprovementDestroyed]]
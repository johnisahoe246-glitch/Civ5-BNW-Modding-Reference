{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered whenever an improvement appears on a player's map &mdash; not when an improvement is created on the general game map. This will be the result of an improvement being created on a tile already been discovered by the active player, or a tile being discovered that already hosts an improvement. Barbarian camps and ancient ruins count as improvements, as indexed in the Improvements table. In the course of building an improvement in the standard game, this event will fire twice, once when the game places the graphic for the improvement in progress of being built, and then again when the improvement is built and the graphic changes to indicate that. The GetImprovementType method on a Plot object, however, will only return improvements that are complete.


=Usage=
<code>'''void''' Events.SerialEventImprovementCreated<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent1, {{Type5|ArtStyleType}} continent2, {{Type5|PlayerID}} player, '''int''' createImprovementType, {{Type5|ImprovementType}} createImprovementRRType, '''int''' createImprovementEra, '''int''' createImprovementState, '''unknown''' ImprovementEra = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventImprovementCreated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventImprovementCreated(''<arguments list>'')</code>.

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
|valign="top"| ''These values appear to always be the same and also seem to refer to the continent on which the improvement was built. Different land masses will have different numbers corresponding to their graphic set, and oceans will be marked as 0.''
|-
|valign="top" style="padding-right:6px;"|continent2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|createImprovementType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|createImprovementRRType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|createImprovementEra:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|createImprovementState:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ImprovementEra:
|valign="top"| ''No description available.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
function onImprovementCreated(iHexX, iHexY, iContinent1, iContinent2)
local pPlot = Map.GetPlot(ToGridFromHex(iHexX, iHexY))
local sImprovement = Map.GetImprovementType() > -1 and GameInfo.Improvements{Map.GetImprovementType()}().Type or "Improvement in progress"
local plotOwner = pPlot:GetOwner() > -1 and Players[pPlot:GetOwner()]:GetName() or "nobody"
print(string.format("%s built on tile %d, %d by player %d. Plot owned by %s", sImprovement, pPlot:GetX(), pPlot:GetY(), iPlayerID, plotOwner))
end
Events.SerialEventImprovementCreated.Add(onImprovementCreated)</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">Events.SerialEventImprovementCreated( iHexX, iHexY, continent,   continent,     playerID,   g_iCreateImprovementType, g_iCreateImprovementRRType, g_iCreateImprovementEra, g_iCreateImprovementState );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2714}}<syntaxhighlight lang="lua">Events.SerialEventImprovementCreated.Add( OnImprovementCreated );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventImprovementCreated]]
[[Category:Civ5 Improvements API|SerialEventImprovementCreated]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered every time a hex is highlighted by the UI. Can be invoked from the Lua side, which highlights a hex and is the common usage. If a highlight style is given, it can be cleared again by using {{Func5|Events|ClearHexHighlightStyle}} or [[Lua_Game_Objects/Events#ClearHexHighlights|ClearHexHighlights]]


=Usage=
<code>'''void''' Events.SerialEventHexHighlight<b>(</b>{{Type5|Vector2}} hex, '''bool''' highlight, {{Type5|Vector4}} highlightColor, '''string''' highlightStyle<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventHexHighlight.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventHexHighlight(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hex:
|valign="top"| ''Hex coordinates of the tile to highlight. Can be created by using the Vector2(iHexX, iHexY) constructor when including FLuaVector.lua (see example)''
|-
|valign="top" style="padding-right:6px;"|highlight:
|valign="top"| ''If true, highlight, if false, remove highlight''
|-
|valign="top" style="padding-right:6px;"|highlightColor:
|valign="top"| ''The color to highlight in. Can be created by using the Vector4(r, g, b, a) constructor when including FLuaVector.lua (see example). Only allows certain colors. Known colors to work: (1,0,0,1), (0,1,0,1), (0,0,1,1), (0,0,1,0.25), (1,1,0,1), (1,0,1,1), (0.5,0.5,0.5,1)''
|-
|valign="top" style="padding-right:6px;"|highlightStyle:
|valign="top"| ''Use a custom highlighting style, in which case highlightColor is irrelevant. Known highlighting styles are: "MovementRangeBorder", "AMRBorder", "FireRangeBorder", "ValidFireTargetBorder", "GroupBorder"''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
include( "FLuaVector" );
-- highlight a hex when it changes ownership
function onHexCultureChanged(iHexX, iHexY, iPlayerID, bUnknown)
Events.SerialEventHexHighlight(Vector2(iHexX, iHexY), true, Vector4(1, 0.5, 0, 1))
end
Events.SerialEventHexCultureChanged.Add(onHexCultureChanged)</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, highlightColor, "FireRangeBorder" );</syntaxhighlight>
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, redColor, "ValidFireTargetBorder");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1824}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( ToHexFromGrid( Vector2( plot:GetX(), plot:GetY() ) ), false, Vector4( 0.0, 1.0, 0.0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1861}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( ToHexFromGrid( Vector2( aPurchasablePlots[i]:GetX(), aPurchasablePlots[i]:GetY() ) ), true, Vector4( 1.0, 0.0, 1.0, 1 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( g_iHexX, g_iHexY ), false, Vector4( 0.5, 0.5, 0.5, 1.0 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( g_iHexX, g_iHexY ), true, Vector4( 0.5, 0.5, 0.5, 1.0 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, false, workerSuggestHighlightColor, genericUnitHexBorder );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, Vector4( 1.0, 1.0, 0.0, 1 ), genericUnitHexBorder );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, embarkColor, genericUnitHexBorder );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, upgradeColor, genericUnitHexBorder );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0558}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, turn2Color, "GroupBorder" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, turn1Color, pathBorderStyle );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0689}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( iHexID, true, vGiftTileImprovementColor, genericUnitHexBorder );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0765}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( i, j ), true, turn1Color, attackPathBorderStyle );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0767}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( i, j ), true, turn1Color, pathBorderStyle );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventHexHighlight]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("FLuaVector.lua")</code>
}}


=Usage=
<code>{{Type5|Vector2}} Vector2<b>(</b>'''float''' i, '''float''' j<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|j:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">local hex = ToHexFromGrid( Vector2(pPlot:GetX(), pPlot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">local nullOffset = Vector2( 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1252}}<syntaxhighlight lang="lua">OnCityCreated( ToHexFromGrid( Vector2( city:GetX(), city:GetY() ) ), player:GetID(), city:GetID() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0614}}<syntaxhighlight lang="lua">local hex = ToHexFromGrid(Vector2(pPlot:GetX(), pPlot:GetY()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1729}}<syntaxhighlight lang="lua">local hexPos = ToHexFromGrid( Vector2( plot:GetX(), plot:GetY() ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1824}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( ToHexFromGrid( Vector2( plot:GetX(), plot:GetY() ) ), false, Vector4( 0.0, 1.0, 0.0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1861}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( ToHexFromGrid( Vector2( aPurchasablePlots[i]:GetX(), aPurchasablePlots[i]:GetY() ) ), true, Vector4( 1.0, 0.0, 1.0, 1 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2601}}<syntaxhighlight lang="lua">local defaultPromotionPortraitOffset = Vector2( 256, 256 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0381}}<syntaxhighlight lang="lua">Events.SerialEventCameraOut( Vector2(0.5,0.5) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0386}}<syntaxhighlight lang="lua">Events.SerialEventCameraIn( Vector2(0.5,0.5) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( g_iHexX, g_iHexY ), false, Vector4( 0.5, 0.5, 0.5, 1.0 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( g_iHexX, g_iHexY ), true, Vector4( 0.5, 0.5, 0.5, 1.0 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">return Vector2( (offset % numCols) * iconSize, math.floor(offset / numCols) * iconSize ), filename;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0304}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( v.plot:GetX(), v.plot:GetY() ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0313}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( v:GetX(), v:GetY() ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0422}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( unit:GetX(), unit:GetY() ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0463}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( evalPlotX, evalPlotY ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0489}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( adjacentPlot:GetX(), adjacentPlot:GetY() ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0555}}<syntaxhighlight lang="lua">local hexID = ToHexFromGrid( Vector2( plotX, plotY) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0688}}<syntaxhighlight lang="lua">local iHexID = ToHexFromGrid( Vector2( iPlotX, iPlotY) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(72,72));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(72,0));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">startPipe.TechPipeIcon:SetSize(   Vector2(40, 42) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(0,72));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">pipe.TechPipeIcon:SetTextureOffset(Vector2(0,0));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0471}}<syntaxhighlight lang="lua">local hex = ToHexFromGrid( Vector2(plot:GetX(), plot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">local GarrisonOffset = Vector2( -43, -39 );</syntaxhighlight>
{{CodeLine5|0021}}<syntaxhighlight lang="lua">local GarrisonOtherOffset = Vector2( -55, -34 );</syntaxhighlight>
{{CodeLine5|0022}}<syntaxhighlight lang="lua">local CityNonGarrisonOffset = Vector2( 45, -45 );</syntaxhighlight>
{{CodeLine5|0023}}<syntaxhighlight lang="lua">local CivilianOffset = Vector2( 0, -15 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0846}}<syntaxhighlight lang="lua">local offset = Vector2( 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">local CivilianOffset = Vector2( 0, -25 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">Events.SerialEventCameraOut( Vector2(0,0) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">Events.SerialEventCameraIn( Vector2(0,0) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0765}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( i, j ), true, turn1Color, attackPathBorderStyle );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0767}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( Vector2( i, j ), true, turn1Color, pathBorderStyle );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Vector2]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>{{Type5|Vector2}} ToHexFromGrid<b>(</b>{{Type5|Vector2}} gridPos<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|gridPos:
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


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0471}}<syntaxhighlight lang="lua">local hex = ToHexFromGrid( Vector2(plot:GetX(), plot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0747}}<syntaxhighlight lang="lua">local hexPosition = ToHexFromGrid(unitPosition);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ToHexFromGrid]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("FLuaVector.lua")</code>
}}


=Usage=
<code>{{Type5|Vector4}} Vector4<b>(</b>'''float''' i, '''float''' j = nil, '''float''' k = nil, '''float''' l = nil<b>)</b></code>


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
|-
|valign="top" style="padding-right:6px;"|k:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|l:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0004}}<syntaxhighlight lang="lua">local redColor = Vector4( 0.7, 0, 0, 1 );</syntaxhighlight>
{{CodeLine5|0005}}<syntaxhighlight lang="lua">local highlightColor = Vector4( 0.7, 0.7, 0, 1 ); -- depending on the theme these may not actually be used (for example SplineBorder do not)</syntaxhighlight>
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


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0428}}<syntaxhighlight lang="lua">local color = Vector4(primaryColor.x, primaryColor.y, primaryColor.z, 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FLuaVector.lua}}
:<code>Gameplay/Lua/FLuaVector.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">function Color( r, g, b, a )   return Vector4( r, g, b, a ); end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">local primaryColorVector = Vector4( primaryColor.Red, primaryColor.Green, primaryColor.Blue, primaryColor.Alpha );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">local secondaryColorVector = Vector4( secondaryColor.Red, secondaryColor.Green, secondaryColor.Blue, secondaryColor.Alpha );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">local primaryColorVector   = Vector4( primaryColor.Red, primaryColor.Green, primaryColor.Blue, primaryColor.Alpha );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0189}}<syntaxhighlight lang="lua">local secondaryColorVector   = Vector4( secondaryColor.Red, secondaryColor.Green, secondaryColor.Blue, secondaryColor.Alpha );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">local workerSuggestHighlightColor = Vector4( 0.0, 0.5, 1.0, 0.65 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">local giftUnitColor = Vector4( 1.0, 1.0, 0.0, 0.65 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">Events.SerialEventHexHighlight( hexID, true, Vector4( 1.0, 1.0, 0.0, 1 ), genericUnitHexBorder );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0430}}<syntaxhighlight lang="lua">local embarkColor = Vector4( 1.0, 1.0, 0.0, 0.65 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0473}}<syntaxhighlight lang="lua">local upgradeColor = Vector4( 0.0, 1.0, 0.5, 0.65 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0658}}<syntaxhighlight lang="lua">local vGiftTileImprovementColor = Vector4( 1.0, 0.0, 1.0, 1.0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetFGColor( Vector4( 0, 1, 0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetFGColor( Vector4( 1, 1, 0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0409}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetFGColor( Vector4( 1, 0, 0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">local worldPos = Vector4( GridToWorld( pPlot:GetX(), pPlot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">o:SetTargetColor( Vector4(0.5, 0.5, 0.5, 1.0) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0367}}<syntaxhighlight lang="lua">member:SetTargetColor( Vector4(0.5, 0.5, 0.5, 1.0) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">g_TargetColors[0] = Vector4(1.0, 0.0, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0596}}<syntaxhighlight lang="lua">g_TargetColors[1] = Vector4(1.0, 1.0, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0597}}<syntaxhighlight lang="lua">g_TargetColors[2] = Vector4(0.5, 1.0, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0598}}<syntaxhighlight lang="lua">g_TargetColors[3] = Vector4(0.0, 1.0, 1.0, 1.0);</syntaxhighlight>
{{CodeLine5|0599}}<syntaxhighlight lang="lua">g_TargetColors[4] = Vector4(0.5, 0.5, 1.0, 1.0);</syntaxhighlight>
{{CodeLine5|0600}}<syntaxhighlight lang="lua">g_TargetColors[5] = Vector4(1.0, 0.5, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0601}}<syntaxhighlight lang="lua">g_TargetColors[6] = Vector4(0.0, 1.0, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0602}}<syntaxhighlight lang="lua">g_TargetColors[7] = Vector4(0.0, 0.0, 1.0, 1.0);</syntaxhighlight>
{{CodeLine5|0603}}<syntaxhighlight lang="lua">g_TargetColors[8] = Vector4(0.5, 0.0, 1.0, 1.0);</syntaxhighlight>
{{CodeLine5|0604}}<syntaxhighlight lang="lua">g_TargetColors[9] = Vector4(0.5, 0.0, 0.5, 1.0);</syntaxhighlight>
{{CodeLine5|0605}}<syntaxhighlight lang="lua">g_TargetColors[10] = Vector4(0.5, 0.25, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0606}}<syntaxhighlight lang="lua">g_TargetColors[11] = Vector4(0.0, 0.25, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0607}}<syntaxhighlight lang="lua">g_TargetColors[12] = Vector4(0.5, 0.0, 0.0, 1.0);</syntaxhighlight>
{{CodeLine5|0608}}<syntaxhighlight lang="lua">g_TargetColors[13] = Vector4(0.25, 0.5, 0.5, 1.0);</syntaxhighlight>
{{CodeLine5|0609}}<syntaxhighlight lang="lua">g_TargetColors[14] = Vector4(0.0, 0.0, 0.5, 1.0);</syntaxhighlight>
{{CodeLine5|0610}}<syntaxhighlight lang="lua">g_TargetColors[15] = Vector4(0.5, 0.0, 0.25, 1.0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local turn1Color = Vector4( 0, 1, 0, 0.25 );</syntaxhighlight>
{{CodeLine5|0007}}<syntaxhighlight lang="lua">local turn2Color = Vector4( 1, 1, 0, 0.25 );</syntaxhighlight>
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local turn3PlusColor = Vector4( 0.25, 0, 1, 0.25 );</syntaxhighlight>
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local maxRangeColor = Vector4( 1, 1, 1, 0.25 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Vector4]]
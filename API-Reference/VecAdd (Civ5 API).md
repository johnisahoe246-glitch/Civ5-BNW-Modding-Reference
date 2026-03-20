{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("FLuaVector.lua")</code>
}}


=Usage=
<code>'''unknown''' VecAdd<b>(</b>'''unknown''' v1, '''unknown''' v2<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|v1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|v2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0639}}<syntaxhighlight lang="lua">controlTable.Anchor:SetWorldPosition( VecAdd( HexPos, WorldPositionOffset ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0727}}<syntaxhighlight lang="lua">controlTable.Anchor:SetWorldPosition( VecAdd( worldPos, WorldPositionOffset ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1735}}<syntaxhighlight lang="lua">controlTable.PlotButtonAnchor:SetWorldPosition( VecAdd( worldPos, WorldPositionOffset ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1840}}<syntaxhighlight lang="lua">controlTable.BuyPlotButtonAnchor:SetWorldPosition( VecAdd( worldPos, WorldPositionOffset2 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0860}}<syntaxhighlight lang="lua">offset = VecAdd( offset, CivilianOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0921}}<syntaxhighlight lang="lua">local position = VecAdd( unitPosition, worldOffset );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1043}}<syntaxhighlight lang="lua">cityFlagInstance.Anchor:SetWorldPosition( VecAdd( worldPos, CityWorldPositionOffset ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0137}}<syntaxhighlight lang="lua">local position = VecAdd( Vector3( worldPosX, worldPosY, worldPosZ ), worldOffset );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|VecAdd]]
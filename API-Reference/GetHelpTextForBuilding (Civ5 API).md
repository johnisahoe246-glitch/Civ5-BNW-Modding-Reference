{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("InfoTooltipInclude.lua")</code>
}}


=Usage=
<code>'''string''' GetHelpTextForBuilding<b>(</b>{{Type5|BuildingType}} building, '''bool''' excludeName, '''bool''' excludeHeader, '''bool''' noMaintenance<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|excludeName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|excludeHeader:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|noMaintenance:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0483}}<syntaxhighlight lang="lua">local strToolTip = GetHelpTextForBuilding(buildingID, bExcludeName, bExcludeHeader, bNoMaintenance);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0866}}<syntaxhighlight lang="lua">szHelpText = GetHelpTextForBuilding(buildingProduction, bExcludeName, bExcludeHeader, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0487}}<syntaxhighlight lang="lua">local strToolTip = GetHelpTextForBuilding(buildingID, bExcludeName, bExcludeHeader, bNoMaintenance, pCity);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0875}}<syntaxhighlight lang="lua">szHelpText = GetHelpTextForBuilding(buildingProduction, bExcludeName, bExcludeHeader, false, pCity);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0563}}<syntaxhighlight lang="lua">strToolTip = Locale.ConvertTextKey(GetHelpTextForBuilding(buildingProduction, false, false, false)) .. "[NEWLINE][NEWLINE]" .. strToolTip;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0976}}<syntaxhighlight lang="lua">strToolTip = GetHelpTextForBuilding(id, bExcludeName, bExcludeHeader, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0651}}<syntaxhighlight lang="lua">strToolTip = Locale.ConvertTextKey(GetHelpTextForBuilding(buildingProduction, false, false, false, city)) .. "[NEWLINE][NEWLINE]" .. strToolTip;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1068}}<syntaxhighlight lang="lua">strToolTip = GetHelpTextForBuilding(id, bExcludeName, bExcludeHeader, false, pCity);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua}}
:<code>UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0368}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( GetHelpTextForBuilding(thisBuildingInfo.ID, bExcludeName, bExcludeHeader, false) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0413}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( GetHelpTextForBuilding(thisBuildingInfo.ID, bExcludeName, bExcludeHeader, false, nil) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UniqueBonuses.lua}}
:<code>UI/FrontEnd/GameSetup/UniqueBonuses.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0048}}<syntaxhighlight lang="lua">thisButton:SetToolTipString( Locale.ConvertTextKey(GetHelpTextForBuilding(thisBuildingInfo.ID, false, false, false)));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">strGameInfo = GetHelpTextForBuilding(iBuildingID, bExcludeName, bExcludeHeader, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHelpTextForBuilding]]
[[Category:Civ5 Buildings API|GetHelpTextForBuilding]]
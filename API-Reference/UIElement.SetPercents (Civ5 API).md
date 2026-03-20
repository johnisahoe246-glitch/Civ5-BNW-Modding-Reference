{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetPercents<b>(</b>'''float''' productionProgressPercent, '''float''' productionProgressPlusThisTurnPercent<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|productionProgressPercent:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|productionProgressPlusThisTurnPercent:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0437}}<syntaxhighlight lang="lua">Controls.EndTurnTimeMeter:SetPercents( percentComplete, percentComplete );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0476}}<syntaxhighlight lang="lua">Controls.AgentActivityProgress:SetPercents( progresspct, nextprogresspct );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0663}}<syntaxhighlight lang="lua">agentEntry.AgentActivityProgress:SetPercents( progresspct, nextprogresspct );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1000}}<syntaxhighlight lang="lua">potentialMeter:SetPercents(pct,pct);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0620}}<syntaxhighlight lang="lua">Controls.ProductionMeter:SetPercents( fProductionProgressPercent, fProductionProgressPlusThisTurnPercent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">Controls.ResearchMeter:SetPercents( fResearchProgressPercent, fResearchProgressPlusThisTurnPercent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">Controls.ResearchMeter:SetPercents( 1, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0186}}<syntaxhighlight lang="lua">thisTechButtonInstance.ProgressMeterInternal:SetPercents( researchProgressPercent, researchProgressPlusThisTurnPercent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPercents]]
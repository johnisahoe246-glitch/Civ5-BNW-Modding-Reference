{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsCity<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">if (plot:GetTeam() == eRivalTeam and (not Teams[eRivalTeam]:IsMinorCiv() or plot:IsCity())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1805}}<syntaxhighlight lang="lua">if (pPlot:IsCity()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">if (plot:IsCity()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">if (pVaticanPlot:IsCity()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0485}}<syntaxhighlight lang="lua">if (pJerusalemPlot:IsCity()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">if( pPlot:IsCity() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0854}}<syntaxhighlight lang="lua">elseif plot:IsCity() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1034}}<syntaxhighlight lang="lua">if( cargoCount > 0 and pPlot:IsCity() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0957}}<syntaxhighlight lang="lua">if (unit:GetDomainType() == DomainTypes.DOMAIN_AIR and not pPlot:IsCity()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCity]]
[[Category:Civ5 Cities API|IsCity]]
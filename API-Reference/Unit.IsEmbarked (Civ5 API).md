{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsEmbarked<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">elseif (not pUnit:IsEmbarked()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1796}}<syntaxhighlight lang="lua">if (pHeadUnit:IsCombatUnit() and (pHeadUnit:IsRanged() and pHeadUnit:IsEmbarked()) == false) and ((pHeadUnit:IsRanged() and pHeadUnit:IsRangeAttackOnlyInDomain() and not pPlot:IsWater()) == false) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1861}}<syntaxhighlight lang="lua">elseif(pHeadUnit:IsRanged() == true and pHeadUnit:IsEmbarked() == false) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0631}}<syntaxhighlight lang="lua">if (pTheirUnit:IsEmbarked()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2086}}<syntaxhighlight lang="lua">if (pHeadUnit:GetDomainType() == pUnit:GetDomainType() or pHeadUnit:IsRanged() or (pHeadUnit:GetDomainType() == DomainTypes.DOMAIN_SEA and pUnit:IsEmbarked())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">if unit:IsEmbarked() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">if( unit:IsEmbarked() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0308}}<syntaxhighlight lang="lua">if (unit:IsEmbarked()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0500}}<syntaxhighlight lang="lua">if( pUnit:IsEmbarked() )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">if( pUnit:IsCombatUnit() and not pUnit:IsEmbarked()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">o.m_IsCivilian = not pUnit:IsCombatUnit() or pUnit:IsEmbarked();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">elseif (not unit:IsEmbarked()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsEmbarked]]
[[Category:Civ5 Movement API|IsEmbarked]]
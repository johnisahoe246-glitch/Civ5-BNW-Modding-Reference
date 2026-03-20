{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsCombatUnit<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1106}}<syntaxhighlight lang="lua">if (pTheirUnit:IsCombatUnit()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1455}}<syntaxhighlight lang="lua">if (theirUnit:IsCombatUnit()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1796}}<syntaxhighlight lang="lua">if (pHeadUnit:IsCombatUnit() and (pHeadUnit:IsRanged() and pHeadUnit:IsEmbarked()) == false) and ((pHeadUnit:IsRanged() and pHeadUnit:IsRangeAttackOnlyInDomain() and not pPlot:IsWater()) == false) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">if( unit:IsCombatUnit() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">if (unit:IsCombatUnit() and unit:GetOriginalOwner() == iCSPlayer) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">if (unit:IsCombatUnit()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">if (pUnit:WorkRate() > 0 and not pUnit:IsCombatUnit() and pUnit:GetDomainType() == DomainTypes.DOMAIN_LAND and pUnit:GetSpecialUnitType() == -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">if (v:IsCombatUnit() and pPlot:GetOwner() == v:GetOwner()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1553}}<syntaxhighlight lang="lua">local bCombatUnit = v:IsCombatUnit();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1557}}<syntaxhighlight lang="lua">local bCombatSecondUnit = w:IsCombatUnit();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1773}}<syntaxhighlight lang="lua">if (v:IsCombatUnit() and not v:IsBusy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1791}}<syntaxhighlight lang="lua">if (v:IsCombatUnit()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3091}}<syntaxhighlight lang="lua">if (v:IsSelected() and not v:IsBusy() and v:GetSpecialUnitType() ~= -1 and not v:IsCombatUnit() and v:GetUnitClassType() ~= ggUnitClassID and v:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">if( pUnit:IsCombatUnit() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">o.m_IsCivilian = not pUnit:IsCombatUnit();</syntaxhighlight>
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
{{CodeLine5|0419}}<syntaxhighlight lang="lua">if unit:IsCombatUnit() or unit:GetDomainType() == DomainTypes.DOMAIN_AIR then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCombatUnit]]
[[Category:Civ5 Units API|IsCombatUnit]]
[[Category:Civ5 Combat API|IsCombatUnit]]
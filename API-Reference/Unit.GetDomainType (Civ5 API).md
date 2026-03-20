{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|DomainType}} Unit:GetDomainType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">if thingThatCanActuallyFire:GetDomainType() == DomainTypes.DOMAIN_LAND and pTargetPlot:IsWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">elseif thingThatCanActuallyFire:GetDomainType() == DomainTypes.DOMAIN_SEA and not pTargetPlot:IsWater() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">if(pUnit:GetDomainType() == DomainTypes.DOMAIN_AIR) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">if(pUnit:GetDomainType() ~= DomainTypes.DOMAIN_AIR) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0602}}<syntaxhighlight lang="lua">if (iTheirStrength == 0 or pTheirUnit:GetDomainType() == DomainTypes.DOMAIN_SEA) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0921}}<syntaxhighlight lang="lua">iModifier = pMyUnit:DomainModifier(pTheirUnit:GetDomainType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1273}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:DomainModifier(pMyUnit:GetDomainType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1838}}<syntaxhighlight lang="lua">if (pHeadUnit:GetDomainType() == pUnit:GetDomainType() or pHeadUnit:IsRanged()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1939}}<syntaxhighlight lang="lua">if (theirUnit:GetDomainType() ~= DomainTypes.DOMAIN_AIR) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0792}}<syntaxhighlight lang="lua">if (not pToPlot:IsWater() and pMyUnit:GetPlot():IsWater() and pMyUnit:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0810}}<syntaxhighlight lang="lua">if (pMyUnit:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1267}}<syntaxhighlight lang="lua">if (pTheirUnit:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1692}}<syntaxhighlight lang="lua">if (theirUnit:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2086}}<syntaxhighlight lang="lua">if (pHeadUnit:GetDomainType() == pUnit:GetDomainType() or pHeadUnit:IsRanged() or (pHeadUnit:GetDomainType() == DomainTypes.DOMAIN_SEA and pUnit:IsEmbarked())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">if (pUnit:WorkRate() > 0 and not pUnit:IsCombatUnit() and pUnit:GetDomainType() == DomainTypes.DOMAIN_LAND and pUnit:GetSpecialUnitType() == -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1635}}<syntaxhighlight lang="lua">if (v:IsRanged() and v:GetDomainType() == DomainTypes.DOMAIN_LAND and v:IsSelected()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1650}}<syntaxhighlight lang="lua">if (v:IsRanged() and v:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2267}}<syntaxhighlight lang="lua">if (v:GetDomainType() == DomainTypes.DOMAIN_SEA and v:IsCanAttack()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2318}}<syntaxhighlight lang="lua">if (v:GetDomainType() == DomainTypes.DOMAIN_SEA and v:WorkRate() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2369}}<syntaxhighlight lang="lua">if (v:GetDomainType() == DomainTypes.DOMAIN_LAND and v:IsCanAttack() and v:IsMustSetUpToRangedAttack()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3091}}<syntaxhighlight lang="lua">if (v:IsSelected() and not v:IsBusy() and v:GetSpecialUnitType() ~= -1 and not v:IsCombatUnit() and v:GetUnitClassType() ~= ggUnitClassID and v:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0083}}<syntaxhighlight lang="lua">if( pUnit:GetDomainType() == DomainTypes.DOMAIN_AIR ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0572}}<syntaxhighlight lang="lua">if (pUnit:GetDomainType() == DomainTypes.DOMAIN_AIR) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1028}}<syntaxhighlight lang="lua">if( pPlotUnit:GetDomainType() == DomainTypes.DOMAIN_AIR ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">if unit:IsCombatUnit() or unit:GetDomainType() == DomainTypes.DOMAIN_AIR then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0587}}<syntaxhighlight lang="lua">if unit:GetDomainType() == DomainTypes.DOMAIN_AIR then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0616}}<syntaxhighlight lang="lua">if(unit:GetDomainType() == DomainTypes.DOMAIN_AIR) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0631}}<syntaxhighlight lang="lua">if(unit:GetDomainType() ~= DomainTypes.DOMAIN_AIR) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0957}}<syntaxhighlight lang="lua">if (unit:GetDomainType() == DomainTypes.DOMAIN_AIR and not pPlot:IsCity()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0629}}<syntaxhighlight lang="lua">if (pHeadSelectedUnit:GetDomainType() == DomainTypes.DOMAIN_AIR) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0646}}<syntaxhighlight lang="lua">if (not cityOwner:IsMinorCiv() and city:GetGarrisonedUnit() == nil and pHeadSelectedUnit:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDomainType]]
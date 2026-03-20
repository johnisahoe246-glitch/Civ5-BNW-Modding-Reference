{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsRanged<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1796}}<syntaxhighlight lang="lua">if (pHeadUnit:IsCombatUnit() and (pHeadUnit:IsRanged() and pHeadUnit:IsEmbarked()) == false) and ((pHeadUnit:IsRanged() and pHeadUnit:IsRangeAttackOnlyInDomain() and not pPlot:IsWater()) == false) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1838}}<syntaxhighlight lang="lua">if (pHeadUnit:GetDomainType() == pUnit:GetDomainType() or pHeadUnit:IsRanged()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1840}}<syntaxhighlight lang="lua">if (pUnit:GetBaseCombatStrength() > 0 or pHeadUnit:IsRanged()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1861}}<syntaxhighlight lang="lua">elseif(pHeadUnit:IsRanged() == true and pHeadUnit:IsEmbarked() == false) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2086}}<syntaxhighlight lang="lua">if (pHeadUnit:GetDomainType() == pUnit:GetDomainType() or pHeadUnit:IsRanged() or (pHeadUnit:GetDomainType() == DomainTypes.DOMAIN_SEA and pUnit:IsEmbarked())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1635}}<syntaxhighlight lang="lua">if (v:IsRanged() and v:GetDomainType() == DomainTypes.DOMAIN_LAND and v:IsSelected()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1650}}<syntaxhighlight lang="lua">if (v:IsRanged() and v:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsRanged]]
[[Category:Civ5 Combat API|IsRanged]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|UnitClassType}} Unit:GetUnitClassType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0891}}<syntaxhighlight lang="lua">iModifier = pMyUnit:GetUnitClassModifier(pTheirUnit:GetUnitClassType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0894}}<syntaxhighlight lang="lua">local unitClassType = Locale.ConvertTextKey(GameInfo.UnitClasses[pTheirUnit:GetUnitClassType()].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0900}}<syntaxhighlight lang="lua">iModifier = pMyUnit:UnitClassAttackModifier(pTheirUnit:GetUnitClassType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1232}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:UnitClassDefenseModifier(pMyUnit:GetUnitClassType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1235}}<syntaxhighlight lang="lua">local unitClassBonus = Locale.ConvertTextKey(GameInfo.UnitClasses[pMyUnit:GetUnitClassType()].Description);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2652}}<syntaxhighlight lang="lua">if(v:GetUnitClassType() == ggUnitClassID) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3091}}<syntaxhighlight lang="lua">if (v:IsSelected() and not v:IsBusy() and v:GetSpecialUnitType() ~= -1 and not v:IsCombatUnit() and v:GetUnitClassType() ~= ggUnitClassID and v:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialInclude_Expansion1.lua (G&K)}}
:<code>DLC/Expansion/Tutorial/TutorialInclude_Expansion1.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">if(unit:GetUnitClassType() == unitClassProphetID) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnitClassType]]
[[Category:Civ5 Units API|GetUnitClassType]]
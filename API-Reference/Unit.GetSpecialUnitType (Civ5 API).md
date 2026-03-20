{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|SpecialUnitType}} Unit:GetSpecialUnitType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">if (pUnit:WorkRate() > 0 and not pUnit:IsCombatUnit() and pUnit:GetDomainType() == DomainTypes.DOMAIN_LAND and pUnit:GetSpecialUnitType() == -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3091}}<syntaxhighlight lang="lua">if (v:IsSelected() and not v:IsBusy() and v:GetSpecialUnitType() ~= -1 and not v:IsCombatUnit() and v:GetUnitClassType() ~= ggUnitClassID and v:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSpecialUnitType]]
[[Category:Civ5 Units API|GetSpecialUnitType]]
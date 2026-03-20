{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:IsBusy<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1244}}<syntaxhighlight lang="lua">if (v:IsCanAttack() and v:IsSelected() and not v:IsBusy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1686}}<syntaxhighlight lang="lua">if (v:CanUpgradeRightNow() and not v:IsBusy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1773}}<syntaxhighlight lang="lua">if (v:IsCombatUnit() and not v:IsBusy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3047}}<syntaxhighlight lang="lua">if (v:IsSelected() and not v:IsBusy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3091}}<syntaxhighlight lang="lua">if (v:IsSelected() and not v:IsBusy() and v:GetSpecialUnitType() ~= -1 and not v:IsCombatUnit() and v:GetUnitClassType() ~= ggUnitClassID and v:GetDomainType() == DomainTypes.DOMAIN_LAND) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsBusy]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsCanAttack<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1244}}<syntaxhighlight lang="lua">if (v:IsCanAttack() and v:IsSelected() and not v:IsBusy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1265}}<syntaxhighlight lang="lua">if (v:IsCanAttack()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2267}}<syntaxhighlight lang="lua">if (v:GetDomainType() == DomainTypes.DOMAIN_SEA and v:IsCanAttack()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2369}}<syntaxhighlight lang="lua">if (v:GetDomainType() == DomainTypes.DOMAIN_LAND and v:IsCanAttack() and v:IsMustSetUpToRangedAttack()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0644}}<syntaxhighlight lang="lua">if (city and city:GetOwner() == pHeadSelectedUnit:GetOwner() and pHeadSelectedUnit:IsCanAttack()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCanAttack]]
[[Category:Civ5 Combat API|IsCanAttack]]
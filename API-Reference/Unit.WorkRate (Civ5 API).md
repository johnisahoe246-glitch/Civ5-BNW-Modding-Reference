{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:WorkRate<b>(</b>'''bool''' max, {{Type5|BuildActionType}} build = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|max:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|build:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">if (pUnit:WorkRate() > 0 and not pUnit:IsCombatUnit() and pUnit:GetDomainType() == DomainTypes.DOMAIN_LAND and pUnit:GetSpecialUnitType() == -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2318}}<syntaxhighlight lang="lua">if (v:GetDomainType() == DomainTypes.DOMAIN_SEA and v:WorkRate() > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1220}}<syntaxhighlight lang="lua">iExtraBuildRate = unit:WorkRate(true, iBuildID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|WorkRate]]
[[Category:Civ5 Units API|WorkRate]]
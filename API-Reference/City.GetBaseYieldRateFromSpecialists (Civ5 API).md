{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetBaseYieldRateFromSpecialists<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|yieldType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0660}}<syntaxhighlight lang="lua">local iYieldFromSpecialists = pCity:GetBaseYieldRateFromSpecialists(iYieldType);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBaseYieldRateFromSpecialists]]
[[Category:Civ5 Yields API|GetBaseYieldRateFromSpecialists]]
[[Category:Civ5 Specialists API|GetBaseYieldRateFromSpecialists]]
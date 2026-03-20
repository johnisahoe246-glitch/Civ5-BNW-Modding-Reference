{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetBaseYieldRateFromReligion<b>(</b>{{Type5|YieldType}} yieldType<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|yieldType:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0740}}<syntaxhighlight lang="lua">local iYieldFromReligion = pCity:GetBaseYieldRateFromReligion(iYieldType);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBaseYieldRateFromReligion]]
[[Category:Civ5 Yields API|GetBaseYieldRateFromReligion]]
[[Category:Civ5 Religion API|GetBaseYieldRateFromReligion]]
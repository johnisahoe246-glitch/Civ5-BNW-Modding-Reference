{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:IsHolyCityForReligion<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1108}}<syntaxhighlight lang="lua">if (city:IsHolyCityForReligion(eReligion)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1142}}<syntaxhighlight lang="lua">if (city:IsHolyCityForReligion(iReligionID)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHolyCityForReligion]]
[[Category:Civ5 Cities API|IsHolyCityForReligion]]
[[Category:Civ5 Religion API|IsHolyCityForReligion]]
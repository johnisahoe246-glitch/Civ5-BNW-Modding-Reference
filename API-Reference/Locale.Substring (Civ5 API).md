{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' Locale.Substring<b>(</b>'''string''' info, '''int''' arg1, '''int''' newLength<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|info:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newLength:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0948}}<syntaxhighlight lang="lua">strInfo = Locale.Substring(strInfo, 1, iNewLength);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SupportFunctions.lua}}
:<code>UI/SupportFunctions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">newString = Locale.Substring(newString, 1, Locale.Length(newString) - 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Substring]]
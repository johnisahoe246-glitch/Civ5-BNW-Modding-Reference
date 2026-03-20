{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


Test if a string ends with a specified suffix (UTF-8 friendly)


=Usage=
<code>'''bool''' Locale.EndsWith<b>(</b>'''string''' base_string, '''string''' suffix<b>)</b></code>


'''Returned Value'''
:Returns true if ''base_string'' ends with ''suffix'', false if otherwise.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|base_string:
|valign="top"| ''The string to test against.''
|-
|valign="top" style="padding-right:6px;"|suffix:
|valign="top"| ''The suffix to use when testing.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local test = Locale.EndsWith("Civilization", "tion");
print(test); -- true</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0946}}<syntaxhighlight lang="lua">if (Locale.EndsWith(strInfo, "[NEWLINE]")) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EndsWith]]
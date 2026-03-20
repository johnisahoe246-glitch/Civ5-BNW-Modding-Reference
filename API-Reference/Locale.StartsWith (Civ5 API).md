{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


Test if a string starts with a specified prefix (UTF-8 friendly)


=Usage=
<code>'''bool''' Locale.StartsWith<b>(</b>'''string''' base_string, '''string''' prefix<b>)</b></code>


'''Returned Value'''
:Returns true if base_string starts with prefix, false otherwise.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|base_string:
|valign="top"| ''The string to test against.''
|-
|valign="top" style="padding-right:6px;"|prefix:
|valign="top"| ''The prefix to test with.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local test = Locale.StartsWith("Civilization", "Civ");
print(test); -- prints true</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|StartsWith]]
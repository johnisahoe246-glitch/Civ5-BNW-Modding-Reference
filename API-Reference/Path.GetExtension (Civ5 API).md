{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns the extension of a file
This method returns the extension of a target file.  Returns an empty string if it cannot determine extension.


=Usage=
<code>'''string''' Path.GetExtension<b>(</b>'''string''' path<b>)</b></code>


'''Returned Value'''
:The extension of the file.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|path:
|valign="top"| ''An absolute or relative path to a file.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local ext = Path.GetExtension("foo.bar");
print(ext); -- prints ".bar"</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2319}}<syntaxhighlight lang="lua">local extension = Path.GetExtension(addinPath);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">local extension = Path.GetExtension(filePath);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetExtension]]
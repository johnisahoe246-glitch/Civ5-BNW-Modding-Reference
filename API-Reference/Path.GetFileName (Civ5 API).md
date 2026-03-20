{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Gets the file name in the target path
This method returns the complete filename in a path, including the extension.


=Usage=
<code>'''string''' Path.GetFileName<b>(</b>'''string''' path<b>)</b></code>


'''Returned Value'''
:The filename, including extension or an empty string on error.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|path:
|valign="top"| ''An absolute or relative path to a file.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local path = "C:\\temp\\foo.bar";
print(Path.GetFileName(path)); -- prints "foo.bar"</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFileName]]
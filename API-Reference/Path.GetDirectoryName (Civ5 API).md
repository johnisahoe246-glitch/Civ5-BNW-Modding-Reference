{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns a path to the deepest folder containing the target
When used with paths to files, this method returns the folder containing the file.  When used with paths to directories, this method returns the folder containing the directory.


=Usage=
<code>'''string''' Path.GetDirectoryName<b>(</b>'''string''' path<b>)</b></code>


'''Returned Value'''
:The folder containing the specified file or folder.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|path:
|valign="top"| ''An absolute or relative path to a file or folder.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local fullpath = "C:\\temp\\foo.bar";
local dir = Path.GetDirectoryName(fullpath);
print(dir); -- prints "C:\temp</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDirectoryName]]
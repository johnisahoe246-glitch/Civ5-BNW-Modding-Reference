{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns a path in which all directory seperators are the same
This method receives a path and returns the same path but with all directory separators set to use the character returned in Path.GetDirectorySeperatorChar().


=Usage=
<code>'''string''' Path.NormalizePath<b>(</b>'''string''' path<b>)</b></code>


'''Returned Value'''
:Returns a path which uses the same directory seperator characters.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|path:
|valign="top"| ''An absolute or relative path.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local validPath = "C:\\temp/foo\\bar.txt";
local easierPath = Path.Normalize(validPath);
print(easierPath); --prints "C:\temp\foo\bar.txt"</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|NormalizePath]]
[[Category:Civ5 Movement API|NormalizePath]]
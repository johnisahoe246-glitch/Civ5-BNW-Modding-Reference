{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Gets the character used to seperate directories in a path.
This method returns the character used to seperate directories in a path with ("\").


=Usage=
<code>'''string''' Path.GetDirectorySeparatorChar<b>(</b><b>)</b></code>


'''Returned Value'''
:The directory seperator character. "\".


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
print(Path.GetDirectorySeperatorChar()); --prints "\"</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDirectorySeparatorChar]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Gets the character used to mark a file extension
This method reutnrs the character used to begin a file extension in a path. "."


=Usage=
<code>'''unknown''' Path.GetExtensionSeparatorChar<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns the extension seperator character. "."


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
print(Path.GetExtensionSeparatorChar()); --prints "."</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetExtensionSeparatorChar]]
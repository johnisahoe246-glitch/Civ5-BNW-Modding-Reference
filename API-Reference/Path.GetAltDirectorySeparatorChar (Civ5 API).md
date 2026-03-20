{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Retrieves an alternate directory separator character
This method retrieves one of the two currently specified directory seperator characters used by paths '/'.


=Usage=
<code>'''string''' Path.GetAltDirectorySeparatorChar<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns an alternate directory separator character. '/


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
print(Path.GetAltDirectorySeperatorChar()); --prints "/"</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetAltDirectorySeparatorChar]]
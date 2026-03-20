{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Path}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns the character used to separate volumes in a path.
This method returns the character used to separate volumes in a path. ":"


=Usage=
<code>'''string''' Path.GetVolumeSeparatorChar<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns the volume separator character. ":".


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
print(Path.GetVolumeSeparatorChar()); -- prints ":"</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetVolumeSeparatorChar]]
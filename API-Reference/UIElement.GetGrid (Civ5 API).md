{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|PullDown}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:GetGrid<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">local width, height = dropDown:GetGrid():GetSizeVal();</syntaxhighlight>
{{CodeLine5|0074}}<syntaxhighlight lang="lua">dropDown:GetGrid():SetSizeVal(width, height+100);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGrid]]
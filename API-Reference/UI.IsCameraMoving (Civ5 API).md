{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' UI.IsCameraMoving<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0593}}<syntaxhighlight lang="lua">if (UI.IsCameraMoving() and not Game.GetAllowRClickMovementWhileScrolling()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCameraMoving]]
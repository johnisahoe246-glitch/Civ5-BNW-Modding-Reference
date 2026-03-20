{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetNumWorldWonders<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">if (Game.GetNumWorldWonders() < 2) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumWorldWonders]]
[[Category:Civ5 Buildings API|GetNumWorldWonders]]
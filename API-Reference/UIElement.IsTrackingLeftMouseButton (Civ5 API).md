{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ButtonBase''' and {{Type5|Slider}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' UIElement:IsTrackingLeftMouseButton<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0733}}<syntaxhighlight lang="lua">if (not Controls.MinorCivsSlider:IsTrackingLeftMouseButton()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsTrackingLeftMouseButton]]
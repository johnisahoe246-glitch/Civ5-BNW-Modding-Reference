{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' OptionsManager.IsCivilianYields<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0968}}<syntaxhighlight lang="lua">if (OptionsManager.IsCivilianYields()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0983}}<syntaxhighlight lang="lua">local bDisplayCivilianYields = OptionsManager.IsCivilianYields();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCivilianYields]]
[[Category:Civ5 Yields API|IsCivilianYields]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''', '''int''' OptionsManager.GetMaxResolution<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0005}}<syntaxhighlight lang="lua">local m_maxX, m_maxY = OptionsManager.GetMaxResolution();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1280}}<syntaxhighlight lang="lua">m_maxX, m_maxY = OptionsManager.GetMaxResolution();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMaxResolution]]
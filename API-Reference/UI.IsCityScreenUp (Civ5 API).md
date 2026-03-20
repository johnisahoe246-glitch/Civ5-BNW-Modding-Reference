{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' UI.IsCityScreenUp<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1716}}<syntaxhighlight lang="lua">if (UI.IsCityScreenUp()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">if (pCity ~= nil and UI.IsCityScreenUp()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCityScreenUp]]
[[Category:Civ5 Cities API|IsCityScreenUp]]
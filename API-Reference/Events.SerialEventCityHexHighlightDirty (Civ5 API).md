{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventCityHexHighlightDirty<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventCityHexHighlightDirty.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventCityHexHighlightDirty(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1873}}<syntaxhighlight lang="lua">Events.SerialEventCityHexHighlightDirty.Add(UpdateWorkingHexes);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventCityHexHighlightDirty]]
[[Category:Civ5 Cities API|SerialEventCityHexHighlightDirty]]
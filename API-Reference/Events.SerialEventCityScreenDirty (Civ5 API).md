{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventCityScreenDirty<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventCityScreenDirty.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventCityScreenDirty(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1467}}<syntaxhighlight lang="lua">Events.SerialEventCityScreenDirty.Add(OnCityViewUpdate);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0794}}<syntaxhighlight lang="lua">Events.SerialEventCityScreenDirty.Add( OnDirty );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventCityScreenDirty]]
[[Category:Civ5 Cities API|SerialEventCityScreenDirty]]
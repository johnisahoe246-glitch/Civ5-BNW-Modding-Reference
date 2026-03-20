{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventExitCityScreen<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventExitCityScreen.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventExitCityScreen(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">Events.SerialEventExitCityScreen.Add(CityScreenClosed);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">Events.SerialEventExitCityScreen();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0185}}<syntaxhighlight lang="lua">Events.SerialEventExitCityScreen.Add( OnExitCityScreen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0695}}<syntaxhighlight lang="lua">Events.SerialEventExitCityScreen.Remove(CityScreenClosed);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1067}}<syntaxhighlight lang="lua">Events.SerialEventExitCityScreen.Add( OnClose );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventExitCityScreen]]
[[Category:Civ5 Cities API|SerialEventExitCityScreen]]
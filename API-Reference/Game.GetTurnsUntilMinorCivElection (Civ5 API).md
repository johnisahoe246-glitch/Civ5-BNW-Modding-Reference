{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' Game.GetTurnsUntilMinorCivElection<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1197}}<syntaxhighlight lang="lua">strCityStateTT = strCityStateTT .. Locale.Lookup("TXT_KEY_EO_CITY_STATE_ELECTION", Game.GetTurnsBetweenMinorCivElections(), Game.GetTurnsUntilMinorCivElection());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTurnsUntilMinorCivElection]]
[[Category:Civ5 United Nations API|GetTurnsUntilMinorCivElection]]
[[Category:Civ5 City States API|GetTurnsUntilMinorCivElection]]
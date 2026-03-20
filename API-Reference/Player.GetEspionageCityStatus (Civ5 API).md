{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>table('''int''' => {{Type5|CityEspionageInfo}}) Player:GetEspionageCityStatus<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0952}}<syntaxhighlight lang="lua">local cityStatus = pActivePlayer:GetEspionageCityStatus();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetEspionageCityStatus]]
[[Category:Civ5 Cities API|GetEspionageCityStatus]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendMinorCivEnterTerritory<b>(</b>{{Type5|TeamID}} rivalTeam<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|rivalTeam:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MinorCivEnterTerritoryPopup.lua}}
:<code>UI/InGame/PopupsGeneric/MinorCivEnterTerritoryPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">Network.SendMinorCivEnterTerritory(eRivalTeam);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendMinorCivEnterTerritory]]
[[Category:Civ5 Movement API|SendMinorCivEnterTerritory]]
[[Category:Civ5 City States API|SendMinorCivEnterTerritory]]
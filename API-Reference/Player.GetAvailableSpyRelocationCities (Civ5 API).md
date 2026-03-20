{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' Player:GetAvailableSpyRelocationCities<b>(</b>'''unknown''' agentID<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|agentID:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">local availableCitiesToRelocate = activePlayer:GetAvailableSpyRelocationCities(agentID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetAvailableSpyRelocationCities]]
[[Category:Civ5 Cities API|GetAvailableSpyRelocationCities]]
[[Category:Civ5 Espionnage API|GetAvailableSpyRelocationCities]]
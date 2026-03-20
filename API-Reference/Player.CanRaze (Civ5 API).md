{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:CanRaze<b>(</b>{{Type5|City}} city, '''bool''' arg1 = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1317}}<syntaxhighlight lang="lua">if (not pPlayer:CanRaze(pCity, false)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1319}}<syntaxhighlight lang="lua">if (pPlayer:CanRaze(pCity, true)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PuppetCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/PuppetCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">local bRaze = activePlayer:CanRaze(newCity);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanRaze]]
[[Category:Civ5 Cities API|CanRaze]]
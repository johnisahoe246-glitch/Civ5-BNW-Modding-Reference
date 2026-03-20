{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetUnhappinessForecast<b>(</b>{{Type5|City}} newCity, {{Type5|City}} newCity<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newCity:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newCity:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|PuppetCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/PuppetCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">local iUnhappinessAnnexedCity = activePlayer:GetUnhappinessForecast(newCity, nil);   -- pAssumeCityAnnexed, pAssumeCityPuppeted</syntaxhighlight>
{{CodeLine5|0038}}<syntaxhighlight lang="lua">local iUnhappinessPuppetCity = activePlayer:GetUnhappinessForecast(nil, newCity);      -- pAssumeCityAnnexed, pAssumeCityPuppeted</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PuppetCityPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PopupsGeneric/PuppetCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">iUnhappinessAnnexedCity = activePlayer:GetUnhappinessForecast(nil, newCity);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnhappinessForecast]]
[[Category:Civ5 Happiness API|GetUnhappinessForecast]]
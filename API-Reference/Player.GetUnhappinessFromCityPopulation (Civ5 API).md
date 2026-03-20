{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetUnhappinessFromCityPopulation<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0393}}<syntaxhighlight lang="lua">local iUnhappinessFromPop = Locale.ToNumber( pPlayer:GetUnhappinessFromCityPopulation() / 100, "#.##" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0640}}<syntaxhighlight lang="lua">local unhappinessFromPop = pPlayer:GetUnhappinessFromCityPopulation() - unhappinessFromSpecialists - iUnhappinessFromPupetCities;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnhappinessFromCityPopulation]]
[[Category:Civ5 Cities API|GetUnhappinessFromCityPopulation]]
[[Category:Civ5 Happiness API|GetUnhappinessFromCityPopulation]]
[[Category:Civ5 Food & Population API|GetUnhappinessFromCityPopulation]]
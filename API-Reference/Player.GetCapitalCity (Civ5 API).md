{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|City}} Player:GetCapitalCity<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0779}}<syntaxhighlight lang="lua">local pCity = pPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0466}}<syntaxhighlight lang="lua">controlTable.MinorButton:SetVoid2(  pOtherPlayer:GetCapitalCity() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0550}}<syntaxhighlight lang="lua">local pCapital = pPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0927}}<syntaxhighlight lang="lua">local pCapital = pMyPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1476}}<syntaxhighlight lang="lua">local pCapital = pTheirPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1818}}<syntaxhighlight lang="lua">local pCapital = theirPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0671}}<syntaxhighlight lang="lua">local pCityStateCity = Players[iToPlayer]:GetCapitalCity()</syntaxhighlight>
{{CodeLine5|0672}}<syntaxhighlight lang="lua">if (pCityStateCity == nil) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">local capital = player:GetCapitalCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0863}}<syntaxhighlight lang="lua">capital = pPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1054}}<syntaxhighlight lang="lua">local capital = pPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1559}}<syntaxhighlight lang="lua">pCity = pPlayer:GetCapitalCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1073}}<syntaxhighlight lang="lua">local pCapitalCity = pMinorCiv:GetCapitalCity();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCapitalCity]]
[[Category:Civ5 Cities API|GetCapitalCity]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Unit}} City:GetGarrisonedUnit<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">local garrisonedUnit = city:GetGarrisonedUnit();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1061}}<syntaxhighlight lang="lua">local unit = city:GetGarrisonedUnit();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1637}}<syntaxhighlight lang="lua">if (myCity:GetGarrisonedUnit() ~= nil) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0337}}<syntaxhighlight lang="lua">if (pCity:GetGarrisonedUnit() ~= nil) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGarrisonedUnit]]
[[Category:Civ5 Units API|GetGarrisonedUnit]]
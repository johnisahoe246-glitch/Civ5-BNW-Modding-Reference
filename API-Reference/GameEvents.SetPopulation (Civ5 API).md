{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Triggered whenever any city changes population. At least, as far as we know. Information provided by {{Type5|User:Sseckman}} calls this CitySetPopulation, but the scenario Lua files refer to SetPopulation.


=Usage=
<code>'''void''' GameEvents.SetPopulation<b>(</b>'''int''' x, '''int''' y, '''unknown''' oldPopulation, '''int''' newPopulation<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''Location of city with change in population''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|oldPopulation:
|valign="top"| ''The population of the city before the change''
|-
|valign="top" style="padding-right:6px;"|newPopulation:
|valign="top"| ''The population of the city after the change''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">GameEvents.SetPopulation.Add(function(iX, iY, oldPopulation, newPopulation)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(iX, iY);</syntaxhighlight>
{{CodeLine5|0055}}<syntaxhighlight lang="lua">local city = plot:GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">if (city:IsRazing()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">if (newPopulation > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">if (GenerateTreasureFromRazedCity(Game:GetHandicapType(), city:GetOwner(), city:GetPreviousOwner())) then</syntaxhighlight>
{{CodeLine5|0062}}<syntaxhighlight lang="lua">local player = Players[city:GetOwner()];</syntaxhighlight>
{{CodeLine5|0063}}<syntaxhighlight lang="lua">local iUnitID;</syntaxhighlight>
{{CodeLine5|0064}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_TREASURE"];</syntaxhighlight>
{{CodeLine5|0065}}<syntaxhighlight lang="lua">player:InitUnit (iUnitID, iX, iY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">local text;</syntaxhighlight>
{{CodeLine5|0068}}<syntaxhighlight lang="lua">local heading;</syntaxhighlight>
{{CodeLine5|0069}}<syntaxhighlight lang="lua">text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_TREASURE_RAZED_CITY", city:GetName());</syntaxhighlight>
{{CodeLine5|0070}}<syntaxhighlight lang="lua">heading = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_TREASURE_FOUND");</syntaxhighlight>
{{CodeLine5|0071}}<syntaxhighlight lang="lua">player:AddNotification(NotificationTypes.NOTIFICATION_GENERIC, text, heading);</syntaxhighlight>
{{CodeLine5|0072}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0073}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0074}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0076}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0077}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPopulation]]
[[Category:Civ5 Food & Population API|SetPopulation]]
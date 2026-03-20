{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}} AssignStartingPlots:GetSmallStrategicResourceQuantityValues<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1304}}<syntaxhighlight lang="lua">local uran_amt, horse_amt, oil_amt, iron_amt, coal_amt, alum_amt = self:GetSmallStrategicResourceQuantityValues()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1306}}<syntaxhighlight lang="lua">-- Main loop</syntaxhighlight>
{{CodeLine5|1307}}<syntaxhighlight lang="lua">local current_index = 1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|9442}}<syntaxhighlight lang="lua">local uran_amt, horse_amt, oil_amt, iron_amt, coal_amt, alum_amt = self:GetSmallStrategicResourceQuantityValues()</syntaxhighlight>
{{CodeLine5|9443}}<syntaxhighlight lang="lua">for city_state = 1, self.iNumCityStates do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1155}}<syntaxhighlight lang="lua">local uran_sm, horse_sm, oil_sm, iron_sm, coal_sm, alum_sm = self:GetSmallStrategicResourceQuantityValues()</syntaxhighlight>
{{CodeLine5|1156}}<syntaxhighlight lang="lua">local bonus_multiplier = 1;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSmallStrategicResourceQuantityValues]]
[[Category:Civ5 Resources API|GetSmallStrategicResourceQuantityValues]]
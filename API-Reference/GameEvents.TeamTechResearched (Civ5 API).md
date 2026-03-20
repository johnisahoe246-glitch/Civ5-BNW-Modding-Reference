{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Triggered when a team researches a tech.


=Usage=
<code>'''void''' GameEvents.TeamTechResearched<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''int''' change<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''The ID of the team that has researched.''
|-
|valign="top" style="padding-right:6px;"|tech:
|valign="top"| ''The ID of the tech that has been researched (presumably).''
|-
|valign="top" style="padding-right:6px;"|change:
|valign="top"| ''No idea.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">GameEvents.TeamTechResearched.Add(OnTechResearched);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0522}}<syntaxhighlight lang="lua">GameEvents.TeamTechResearched.Add(function(iTeam, iTech, iChange)</syntaxhighlight>
{{CodeLine5|0523}}<syntaxhighlight lang="lua">local kCultureBonus = GetCultureFromLastTech();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0525}}<syntaxhighlight lang="lua">if (iTech == GameInfo.Technologies["TECH_THE_GRAND_IDEA"].ID) then</syntaxhighlight>
{{CodeLine5|0526}}<syntaxhighlight lang="lua">for iPlayer = 0, GameDefines.MAX_MAJOR_CIVS - 1, 1 do</syntaxhighlight>
{{CodeLine5|0527}}<syntaxhighlight lang="lua">   if (Players[iPlayer] ~= nil) then</syntaxhighlight>
{{CodeLine5|0528}}<syntaxhighlight lang="lua">   if (Players[iPlayer]:GetTeam() == iTeam) then</syntaxhighlight>
{{CodeLine5|0529}}<syntaxhighlight lang="lua">   Players[iPlayer]:ChangeJONSCulture(kCultureBonus);</syntaxhighlight>
{{CodeLine5|0530}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0531}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0532}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0533}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0534}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TeamTechResearched]]
[[Category:Civ5 Science API|TeamTechResearched]]
[[Category:Civ5 Diplomacy API|TeamTechResearched]]
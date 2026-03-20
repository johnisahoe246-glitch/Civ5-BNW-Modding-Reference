{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''void''' GameEvents.PlayerCityFounded<b>(</b>{{Type5|PlayerID}} player, '''int''' cityX, '''int''' cityY<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cityX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cityY:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0510}}<syntaxhighlight lang="lua">GameEvents.PlayerCityFounded.Add(function(iPlayer, iCityX, iCityY)</syntaxhighlight>
{{CodeLine5|0511}}<syntaxhighlight lang="lua">local kCultureBonus = GetCultureFromFirstCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0513}}<syntaxhighlight lang="lua">-- If this is player's first city, grant them the starting Culture amount</syntaxhighlight>
{{CodeLine5|0514}}<syntaxhighlight lang="lua">local pPlayer = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0515}}<syntaxhighlight lang="lua">if (pPlayer ~= nil) then</syntaxhighlight>
{{CodeLine5|0516}}<syntaxhighlight lang="lua">if (not pPlayer:IsMinorCiv() and pPlayer:GetNumCities() == 1) then</syntaxhighlight>
{{CodeLine5|0517}}<syntaxhighlight lang="lua">pPlayer:ChangeJONSCulture(kCultureBonus);</syntaxhighlight>
{{CodeLine5|0518}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0519}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0520}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlayerCityFounded]]
[[Category:Civ5 Cities API|PlayerCityFounded]]
[[Category:Civ5 Players API|PlayerCityFounded]]
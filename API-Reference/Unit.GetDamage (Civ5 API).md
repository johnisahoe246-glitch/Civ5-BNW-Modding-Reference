{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetDamage<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">iMyDamageInflicted = pMyUnit:GetCombatDamage(iMyStrength, iTheirStrength, pMyUnit:GetDamage() + iTheirFireSupportCombatDamage, false, false, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">if (pMyUnit:GetDamage() + iTheirDamageInflicted >= maxUnitHitPoints) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0362}}<syntaxhighlight lang="lua">DoUpdateHealthBars(maxUnitHitPoints, maxCityHitPoints, pMyUnit:GetDamage(), pCity:GetDamage(), iMyDamageInflicted, iTheirDamageInflicted)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">elseif (pMyUnit:GetDamage() > (maxUnitHitPoints / 2) and iTheirDamageInflicted > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0616}}<syntaxhighlight lang="lua">iMyDamageInflicted = pMyUnit:GetCombatDamage(iMyStrength, iTheirStrength, pMyUnit:GetDamage() + iTheirFireSupportCombatDamage, false, false, false);</syntaxhighlight>
{{CodeLine5|0617}}<syntaxhighlight lang="lua">iTheirDamageInflicted = pTheirUnit:GetCombatDamage(iTheirStrength, iMyStrength, pTheirUnit:GetDamage(), false, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">DoUpdateHealthBars(maxUnitHitPoints, maxUnitHitPoints, pMyUnit:GetDamage(), pTheirUnit:GetDamage(), iMyDamageInflicted, iTheirDamageInflicted)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0947}}<syntaxhighlight lang="lua">if (pTheirUnit:GetDamage() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1419}}<syntaxhighlight lang="lua">local theirUnitCurHP = theirUnit:GetDamage();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0303}}<syntaxhighlight lang="lua">if (unit:GetDamage() > 0) then</syntaxhighlight>
{{CodeLine5|0304}}<syntaxhighlight lang="lua">strUnitText = strUnitText .. ", " .. Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_HP", GameDefines["MAX_HIT_POINTS"] - unit:GetDamage());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">iUnitDamage = unit:GetDamage();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0651}}<syntaxhighlight lang="lua">local damage = unit:GetDamage();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDamage]]
[[Category:Civ5 Combat API|GetDamage]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetCombatDamage<b>(</b>'''int''' strength, '''int''' opponentStrength, '''int''' currentDamage, '''bool''' includeRand = true, '''bool''' attackerIsCity = false, '''bool''' defenderIsCity = false<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|strength:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|opponentStrength:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|currentDamage:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|includeRand:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|attackerIsCity:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|defenderIsCity:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">iMyDamageInflicted = pMyUnit:GetCombatDamage(iMyStrength, iTheirStrength, pMyUnit:GetDamage() + iTheirFireSupportCombatDamage, false, false, true);</syntaxhighlight>
{{CodeLine5|0333}}<syntaxhighlight lang="lua">iTheirDamageInflicted = pMyUnit:GetCombatDamage(iTheirStrength, iMyStrength, pCity:GetDamage(), false, true, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0616}}<syntaxhighlight lang="lua">iMyDamageInflicted = pMyUnit:GetCombatDamage(iMyStrength, iTheirStrength, pMyUnit:GetDamage() + iTheirFireSupportCombatDamage, false, false, false);</syntaxhighlight>
{{CodeLine5|0617}}<syntaxhighlight lang="lua">iTheirDamageInflicted = pTheirUnit:GetCombatDamage(iTheirStrength, iMyStrength, pTheirUnit:GetDamage(), false, false, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCombatDamage]]
[[Category:Civ5 Combat API|GetCombatDamage]]
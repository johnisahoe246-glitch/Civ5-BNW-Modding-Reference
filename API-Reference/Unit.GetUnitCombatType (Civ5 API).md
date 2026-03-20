{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|UnitCombatType}} Unit:GetUnitCombatType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0909}}<syntaxhighlight lang="lua">if (pTheirUnit:GetUnitCombatType() ~= -1) then</syntaxhighlight>
{{CodeLine5|0910}}<syntaxhighlight lang="lua">iModifier = pMyUnit:UnitCombatModifier(pTheirUnit:GetUnitCombatType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0914}}<syntaxhighlight lang="lua">local unitClassType = Locale.ConvertTextKey(GameInfo.UnitCombatInfos[pTheirUnit:GetUnitCombatType()].Description);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1249}}<syntaxhighlight lang="lua">if (pMyUnit:GetUnitCombatType() ~= -1) then</syntaxhighlight>
{{CodeLine5|1250}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:UnitCombatModifier(pMyUnit:GetUnitCombatType());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1254}}<syntaxhighlight lang="lua">local unitClassType = Locale.ConvertTextKey(GameInfo.UnitCombatInfos[pMyUnit:GetUnitCombatType()].Description);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnitCombatType]]
[[Category:Civ5 Units API|GetUnitCombatType]]
[[Category:Civ5 Combat API|GetUnitCombatType]]
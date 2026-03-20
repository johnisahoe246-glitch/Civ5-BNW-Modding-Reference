{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|City}} Game.GetHolyCityForReligion<b>(</b>{{Type5|ReligionType}} religion, {{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0494}}<syntaxhighlight lang="lua">local holyCity = Game.GetHolyCityForReligion(eReligion, iPlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">local pOrthodoxHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_ORTHODOXY"], -1);</syntaxhighlight>
{{CodeLine5|0193}}<syntaxhighlight lang="lua">local pIslamHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_ISLAM"], -1);</syntaxhighlight>
{{CodeLine5|0194}}<syntaxhighlight lang="lua">local pChristianityHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_CHRISTIANITY"], -1);</syntaxhighlight>
{{CodeLine5|0195}}<syntaxhighlight lang="lua">local pProtestantHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_PROTESTANTISM"], -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0503}}<syntaxhighlight lang="lua">local pHolyCity = Game.GetHolyCityForReligion(iMyCivsReligion, -1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHolyCityForReligion]]
[[Category:Civ5 Cities API|GetHolyCityForReligion]]
[[Category:Civ5 Religion API|GetHolyCityForReligion]]
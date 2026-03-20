{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetGoldPerTurnFromReligion<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EconomicGeneralInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local religionGPT = pPlayer:GetGoldPerTurnFromReligion();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0462}}<syntaxhighlight lang="lua">local iGoldPerTurnFromReligion = pPlayer:GetGoldPerTurnFromReligion();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGoldPerTurnFromReligion]]
[[Category:Civ5 Religion API|GetGoldPerTurnFromReligion]]
[[Category:Civ5 Gold API|GetGoldPerTurnFromReligion]]
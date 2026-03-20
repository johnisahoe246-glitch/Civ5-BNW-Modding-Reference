{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ReligionType}} City:GetReligiousMajority<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1098}}<syntaxhighlight lang="lua">local eReligion = city:GetReligiousMajority();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">if (pCity:GetReligiousMajority() == GameInfoTypes["RELIGION_ORTHODOXY"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1563}}<syntaxhighlight lang="lua">elseif (pCity:GetReligiousMajority() ~= GameInfoTypes["RELIGION_CHRISTIANITY"]) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetReligiousMajority]]
[[Category:Civ5 Religion API|GetReligiousMajority]]
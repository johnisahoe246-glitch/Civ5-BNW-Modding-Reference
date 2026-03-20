{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Team:Meet<b>(</b>{{Type5|TeamID}} team, '''bool''' newDiplo<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newDiplo:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0983}}<syntaxhighlight lang="lua">pTeam:Meet(vaticanTeamID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1004}}<syntaxhighlight lang="lua">pTeam:Meet(byzantineTeamID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1007}}<syntaxhighlight lang="lua">pTeam:Meet(meccaTeamID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1018}}<syntaxhighlight lang="lua">pTeam:Meet(jerusalemTeamID, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Meet]]
[[Category:Civ5 Diplomacy API|Meet]]
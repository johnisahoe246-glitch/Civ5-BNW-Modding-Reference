{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetFaithPerTurnFromMinorCivs<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local iFaithFromMinorCivs = player:GetFaithPerTurnFromMinorCivs();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0924}}<syntaxhighlight lang="lua">local iFaithFromMinorCivs = pPlayer:GetFaithPerTurnFromMinorCivs();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFaithPerTurnFromMinorCivs]]
[[Category:Civ5 Religion API|GetFaithPerTurnFromMinorCivs]]
[[Category:Civ5 Players API|GetFaithPerTurnFromMinorCivs]]
[[Category:Civ5 City States API|GetFaithPerTurnFromMinorCivs]]
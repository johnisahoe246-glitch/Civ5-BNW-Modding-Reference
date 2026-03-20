{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|BeliefType}} Player:GetBeliefInPantheon<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0393}}<syntaxhighlight lang="lua">local eBelief = pPlayer:GetBeliefInPantheon();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0381}}<syntaxhighlight lang="lua">local iBelief = player:GetBeliefInPantheon();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0592}}<syntaxhighlight lang="lua">local iBelief = pPlayer:GetBeliefInPantheon();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBeliefInPantheon]]
[[Category:Civ5 Religion API|GetBeliefInPantheon]]
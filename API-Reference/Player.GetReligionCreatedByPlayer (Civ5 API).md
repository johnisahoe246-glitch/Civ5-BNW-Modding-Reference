{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ReligionType}} Player:GetReligionCreatedByPlayer<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">local eReligion = pPlayer:GetReligionCreatedByPlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">local eReligion = player:GetReligionCreatedByPlayer();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">if (player:GetReligionCreatedByPlayer() > ReligionTypes.RELIGION_PANTHEON or Game.GetNumReligionsStillToFound() > 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetReligionCreatedByPlayer]]
[[Category:Civ5 Religion API|GetReligionCreatedByPlayer]]
[[Category:Civ5 Players API|GetReligionCreatedByPlayer]]
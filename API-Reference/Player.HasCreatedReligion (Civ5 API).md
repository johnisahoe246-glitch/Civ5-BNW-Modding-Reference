{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:HasCreatedReligion<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_PROPHET"].ID and (not player:HasCreatedPantheon() or (not player:HasCreatedReligion() and Game.GetNumReligionsStillToFound() == 0))) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">if (pPlayer:IsEverAlive() and pPlayer:HasCreatedReligion()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">if (pPlayer:HasCreatedReligion()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0437}}<syntaxhighlight lang="lua">if (not pPlayer:HasCreatedReligion()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">if(player:HasCreatedReligion()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">return (player:HasCreatedReligion() or (player:HasCreatedPantheon() and Game.GetNumReligionsStillToFound() > 0));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">if (player:HasCreatedReligion()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0945}}<syntaxhighlight lang="lua">if (Game.GetNumReligionsStillToFound() > 0 or pPlayer:HasCreatedReligion()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasCreatedReligion]]
[[Category:Civ5 Religion API|HasCreatedReligion]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetNumReligionsStillToFound<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_PROPHET"].ID and (not player:HasCreatedPantheon() or (not player:HasCreatedReligion() and Game.GetNumReligionsStillToFound() == 0))) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">return (player:HasCreatedReligion() or (player:HasCreatedPantheon() and Game.GetNumReligionsStillToFound() > 0));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">if (player:GetReligionCreatedByPlayer() > ReligionTypes.RELIGION_PANTHEON or Game.GetNumReligionsStillToFound() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0552}}<syntaxhighlight lang="lua">local iReligionsLeft = Game.GetNumReligionsStillToFound();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0945}}<syntaxhighlight lang="lua">if (Game.GetNumReligionsStillToFound() > 0 or pPlayer:HasCreatedReligion()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0960}}<syntaxhighlight lang="lua">if (Game.GetNumReligionsStillToFound() < 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0963}}<syntaxhighlight lang="lua">strText = strText .. Locale.ConvertTextKey("TXT_KEY_TP_FAITH_RELIGIONS_LEFT", Game.GetNumReligionsStillToFound());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumReligionsStillToFound]]
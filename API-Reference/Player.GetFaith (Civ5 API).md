{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetFaith<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0119}}<syntaxhighlight lang="lua">local currentFaith = player:GetFaith();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">Controls.CurrentFaith:LocalizeAndSetText("TXT_KEY_RO_FAITH", player:GetFaith(), minFaithForProphet);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">strFaithStr = string.format("%i (+%i)", pPlayer:GetFaith(), pPlayer:GetTotalFaithPerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0913}}<syntaxhighlight lang="lua">strText = strText .. Locale.ConvertTextKey("TXT_KEY_TP_FAITH_ACCUMULATED", pPlayer:GetFaith());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialInclude_Expansion1.lua (G&K)}}
:<code>DLC/Expansion/Tutorial/TutorialInclude_Expansion1.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">if(player:GetFaith() > 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFaith]]
[[Category:Civ5 Religion API|GetFaith]]
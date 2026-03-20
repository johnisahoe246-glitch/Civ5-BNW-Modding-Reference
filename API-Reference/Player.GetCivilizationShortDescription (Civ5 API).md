{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Player:GetCivilizationShortDescription<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">thirdName = pThirdPlayer:GetCivilizationShortDescription();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1289}}<syntaxhighlight lang="lua">CivShortDescription = player:GetCivilizationShortDescription(),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">strVoteCastTT = Locale.ConvertTextKey("TXT_KEY_POP_UN_ELEC_VOTE_TT_CITYSTATE_ALT", pPlayer:GetCivilizationShortDescription(), pVoteCastPlayer:GetCivilizationShortDescription());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">strVoteCastTT = Locale.ConvertTextKey("TXT_KEY_POP_UN_ELEC_VOTE_TT_CIV_ALT", pPlayer:GetCivilizationShortDescription(), pVoteCastPlayer:GetCivilizationShortDescription());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCivilizationShortDescription]]
[[Category:Civ5 Players API|GetCivilizationShortDescription]]
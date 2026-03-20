{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsMinorCivActiveQuestForPlayer<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|major:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|type:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0608}}<syntaxhighlight lang="lua">if (pMinor:IsMinorCivActiveQuestForPlayer(iActivePlayer, MinorCivQuestTypes.MINOR_CIV_QUEST_KILL_CAMP)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0399}}<syntaxhighlight lang="lua">if (pMinor:IsMinorCivActiveQuestForPlayer(iMajor, eType)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0529}}<syntaxhighlight lang="lua">if (pMinor:IsMinorCivActiveQuestForPlayer(g_iPlayer, MinorCivQuestTypes.MINOR_CIV_QUEST_KILL_CAMP)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsMinorCivActiveQuestForPlayer(iActivePlayer, MinorCivQuestTypes.MINOR_CIV_QUEST_KILL_CAMP)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMinorCivActiveQuestForPlayer]]
[[Category:Civ5 Players API|IsMinorCivActiveQuestForPlayer]]
[[Category:Civ5 City States API|IsMinorCivActiveQuestForPlayer]]
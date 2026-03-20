{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetQuestData1<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} type = nil<b>)</b></code>


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

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">local iQuestData1 = pPlayer:GetQuestData1(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">local iQuestData1 = pMinor:GetQuestData1(iActivePlayer, MinorCivQuestTypes.MINOR_CIV_QUEST_KILL_CAMP);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">local iQuestData1 = pMinor:GetQuestData1(iMajor, eType);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0486}}<syntaxhighlight lang="lua">local iQuestData1 = pOtherPlayer:GetQuestData1(g_iPlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">local iQuestData1 = pMinor:GetQuestData1(g_iPlayer, MinorCivQuestTypes.MINOR_CIV_QUEST_KILL_CAMP);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local iQuestData1 = pOtherPlayer:GetQuestData1(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local iQuestData1 = pOtherPlayer:GetQuestData1(iActivePlayer, MinorCivQuestTypes.MINOR_CIV_QUEST_KILL_CAMP);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetQuestData1]]
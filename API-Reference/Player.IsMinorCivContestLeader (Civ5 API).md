{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsMinorCivContestLeader<b>(</b>{{Type5|PlayerID}} major, {{Type5|MinorCivQuestType}} arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|major:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0502}}<syntaxhighlight lang="lua">if (pMinor:IsMinorCivContestLeader(iMajor, MinorCivQuestTypes.MINOR_CIV_QUEST_CONTEST_CULTURE)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0510}}<syntaxhighlight lang="lua">if (pMinor:IsMinorCivContestLeader(iMajor, MinorCivQuestTypes.MINOR_CIV_QUEST_CONTEST_FAITH)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">if (pMinor:IsMinorCivContestLeader(iMajor, MinorCivQuestTypes.MINOR_CIV_QUEST_CONTEST_TECHS)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMinorCivContestLeader]]
[[Category:Civ5 Players API|IsMinorCivContestLeader]]
[[Category:Civ5 City States API|IsMinorCivContestLeader]]
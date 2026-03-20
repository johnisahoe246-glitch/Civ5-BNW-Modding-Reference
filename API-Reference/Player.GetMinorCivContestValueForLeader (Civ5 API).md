{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetMinorCivContestValueForLeader<b>(</b>{{Type5|MinorCivQuestType}} arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0500}}<syntaxhighlight lang="lua">local iLeaderScore = pMinor:GetMinorCivContestValueForLeader(MinorCivQuestTypes.MINOR_CIV_QUEST_CONTEST_CULTURE);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0508}}<syntaxhighlight lang="lua">local iLeaderScore = pMinor:GetMinorCivContestValueForLeader(MinorCivQuestTypes.MINOR_CIV_QUEST_CONTEST_FAITH);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0516}}<syntaxhighlight lang="lua">local iLeaderScore = pMinor:GetMinorCivContestValueForLeader(MinorCivQuestTypes.MINOR_CIV_QUEST_CONTEST_TECHS);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMinorCivContestValueForLeader]]
[[Category:Civ5 Players API|GetMinorCivContestValueForLeader]]
[[Category:Civ5 City States API|GetMinorCivContestValueForLeader]]
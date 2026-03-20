{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsMinorWarQuestWithMajorActive<b>(</b>{{Type5|PlayerID}} playerLoop = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|playerLoop:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0383}}<syntaxhighlight lang="lua">if (pPlayer:IsMinorWarQuestWithMajorActive(iPlayerLoop)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1136}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsMinorWarQuestWithMajorActive()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMinorWarQuestWithMajorActive]]
[[Category:Civ5 Diplomacy API|IsMinorWarQuestWithMajorActive]]
[[Category:Civ5 City States API|IsMinorWarQuestWithMajorActive]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:SetHasPolicy<b>(</b>{{Type5|PolicyType}} index, '''bool''' newValue<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0988}}<syntaxhighlight lang="lua">pPlayer:SetHasPolicy(GameInfo.Policies["POLICY_ROMAN_ATROPHY"].ID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0991}}<syntaxhighlight lang="lua">pPlayer:SetHasPolicy(GameInfo.Policies["POLICY_SASSANID_HERITAGE"].ID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0994}}<syntaxhighlight lang="lua">pPlayer:SetHasPolicy(GameInfo.Policies["POLICY_BARBARIAN_HERITAGE"].ID, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetHasPolicy]]
[[Category:Civ5 Policies API|SetHasPolicy]]
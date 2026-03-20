{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|ReligionType}} Game.GetFounderBenefitsReligion<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">local eFounderBenefitsReligion = Game.GetFounderBenefitsReligion(iPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0386}}<syntaxhighlight lang="lua">local eFounderReligion = Game.GetFounderBenefitsReligion(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFounderBenefitsReligion]]
[[Category:Civ5 Religion API|GetFounderBenefitsReligion]]
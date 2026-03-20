{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''void''' GameEvents.GetReligionToSpread<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0525}}<syntaxhighlight lang="lua">GameEvents.GetReligionToSpread.Add(function(ePlayer)</syntaxhighlight>
{{CodeLine5|0526}}<syntaxhighlight lang="lua">return MyCurrentReligion(ePlayer);</syntaxhighlight>
{{CodeLine5|0527}}<syntaxhighlight lang="lua">end)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0529}}<syntaxhighlight lang="lua">function MyCurrentReligion(ePlayer)</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetReligionToSpread]]
[[Category:Civ5 Religion API|GetReligionToSpread]]
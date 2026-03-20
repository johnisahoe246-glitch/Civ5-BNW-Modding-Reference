{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' GameEvents.PlayerAdoptPolicy<b>(</b>{{Type5|PlayerID}} player, '''int''' policyID<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|policyID:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0467}}<syntaxhighlight lang="lua">GameEvents.PlayerAdoptPolicy.Add(OnPolicyAdopted);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlayerAdoptPolicy]]
[[Category:Civ5 Policies API|PlayerAdoptPolicy]]
[[Category:Civ5 Players API|PlayerAdoptPolicy]]
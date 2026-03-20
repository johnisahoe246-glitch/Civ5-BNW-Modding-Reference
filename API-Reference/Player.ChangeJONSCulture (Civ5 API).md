{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:ChangeJONSCulture<b>(</b>'''int''' change<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|change:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0254}}<syntaxhighlight lang="lua">Players[iPlayer]:ChangeJONSCulture(20 * iCitiesCaptured);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">pPlayer:ChangeJONSCulture(kCultureBonus);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0529}}<syntaxhighlight lang="lua">Players[iPlayer]:ChangeJONSCulture(kCultureBonus);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeJONSCulture]]
[[Category:Civ5 Culture API|ChangeJONSCulture]]
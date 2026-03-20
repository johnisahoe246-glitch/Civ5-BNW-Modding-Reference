{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumPolicies<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0216}}<syntaxhighlight lang="lua">local iValue = Players[iPlayer]:GetNumPolicies();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">if (pLoopPlayer:GetNumPolicies() < 2) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">return pPlayer:GetNumPolicies();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumPolicies]]
[[Category:Civ5 Policies API|GetNumPolicies]]
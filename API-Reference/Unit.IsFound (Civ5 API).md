{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsFound<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1077}}<syntaxhighlight lang="lua">if (pUnit ~= nil and pUnit:IsFound()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">if (v:IsFound() and v:MovesLeft() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1369}}<syntaxhighlight lang="lua">if (v:IsFound()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1502}}<syntaxhighlight lang="lua">if (v:IsFound() and  v:MovesLeft() > 0 and v:IsSelected()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsFound]]
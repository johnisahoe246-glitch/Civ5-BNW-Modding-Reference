{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumMinorCivsMet<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1021}}<syntaxhighlight lang="lua">iLastTurnNumMinorsMet = GetPlayer():GetNumMinorCivsMet();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1027}}<syntaxhighlight lang="lua">dprint("player:GetNumMinorCivsMet(): " .. GetPlayer():GetNumMinorCivsMet());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1040}}<syntaxhighlight lang="lua">if (player:GetNumMinorCivsMet() == 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumMinorCivsMet]]
[[Category:Civ5 Players API|GetNumMinorCivsMet]]
[[Category:Civ5 Diplomacy API|GetNumMinorCivsMet]]
[[Category:Civ5 City States API|GetNumMinorCivsMet]]
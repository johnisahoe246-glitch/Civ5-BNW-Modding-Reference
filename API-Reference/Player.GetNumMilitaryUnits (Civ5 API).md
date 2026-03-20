{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumMilitaryUnits<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0496}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() > 50 or player:GetNumMilitaryUnits() >= 2) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0512}}<syntaxhighlight lang="lua">if (player:GetNumMilitaryUnits() <= player:GetNumCities()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0694}}<syntaxhighlight lang="lua">if (player:GetNumMilitaryUnits() ~= 1) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumMilitaryUnits]]
[[Category:Civ5 Units API|GetNumMilitaryUnits]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsEmpireUnhappy<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">if (not pPlayer:IsEmpireUnhappy()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0546}}<syntaxhighlight lang="lua">elseif (pPlayer:IsEmpireUnhappy()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0870}}<syntaxhighlight lang="lua">if (not player:IsEmpireUnhappy()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsEmpireUnhappy]]
[[Category:Civ5 Happiness API|IsEmpireUnhappy]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetTeam<b>(</b>{{Type5|PlayerID}} player, {{Type5|PlayerID}} playerChoice<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|playerChoice:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0994}}<syntaxhighlight lang="lua">PreGame.SetTeam(playerID, playerChoiceID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1200}}<syntaxhighlight lang="lua">PreGame.SetTeam(i, i);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetTeam]]
[[Category:Civ5 Diplomacy API|SetTeam]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Activates game overlay to specific page


=Usage=
<code>'''void''' Steam.ActivateGameOverlay<b>(</b>'''string''' page<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|page:
|valign="top"| ''A string representing which page of the overlay you'd like to display.
Valid options are: Friends, Community, Players, Settings, LobbyInvite, OfficialGameGroup, Stats, and Achievements.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
--Show achievements
Steam.ActivateGameOverlay("Achievements");</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ActivateGameOverlay]]
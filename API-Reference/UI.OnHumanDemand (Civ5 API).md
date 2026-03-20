{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.OnHumanDemand<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|aIPlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0258}}<syntaxhighlight lang="lua">UI.OnHumanDemand(g_iAIPlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OnHumanDemand]]
[[Category:Civ5 Players API|OnHumanDemand]]
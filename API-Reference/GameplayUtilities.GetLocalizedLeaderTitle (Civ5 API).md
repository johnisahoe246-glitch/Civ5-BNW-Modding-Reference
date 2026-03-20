{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameplayUtilities}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' GameplayUtilities.GetLocalizedLeaderTitle<b>(</b>{{Type5|Player}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">local strTitleText = GameplayUtilities.GetLocalizedLeaderTitle(player);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewTurn.lua}}
:<code>UI/InGame/NewTurn.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">local strInfo = GameplayUtilities.GetLocalizedLeaderTitle(player);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLocalizedLeaderTitle]]
[[Category:Civ5 Players API|GetLocalizedLeaderTitle]]
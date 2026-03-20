{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AILeaderMessage<b>(</b>{{Type5|PlayerID}} player, {{Type5|DiploUIStateType}} diploUIState, '''string''' leaderMessage, '''int''' animationAction, '''int''' data1<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AILeaderMessage.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AILeaderMessage(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|diploUIState:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|leaderMessage:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|animationAction:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|data1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploTrade.lua}}
:<code>UI/InGame/LeaderHead/DiploTrade.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0004}}<syntaxhighlight lang="lua">Events.AILeaderMessage.Add( LeaderMessageHandler );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AILeaderMessage]]
[[Category:Civ5 Players API|AILeaderMessage]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.LeavingLeaderViewMode<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.LeavingLeaderViewMode.Add(''<function handler>'')</code> or invoke it directly through <code>Events.LeavingLeaderViewMode(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploTrade.lua}}
:<code>UI/InGame/LeaderHead/DiploTrade.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">Events.LeavingLeaderViewMode.Add( OnLeavingLeader );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LeavingLeaderViewMode]]
[[Category:Civ5 Players API|LeavingLeaderViewMode]]
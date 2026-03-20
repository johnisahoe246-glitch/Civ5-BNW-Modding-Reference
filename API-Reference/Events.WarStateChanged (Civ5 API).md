{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.WarStateChanged<b>(</b>{{Type5|TeamID}} team1, {{Type5|TeamID}} team2, '''bool''' war<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.WarStateChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.WarStateChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|team2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|war:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">Events.WarStateChanged.Add( WarStateChangedHandler );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|WarStateChanged]]
[[Category:Civ5 Diplomacy API|WarStateChanged]]
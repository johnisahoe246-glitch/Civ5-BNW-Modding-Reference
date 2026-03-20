{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Plot:ChangeVisibilityCount<b>(</b>{{Type5|TeamID}} team, '''int''' change, {{Type5|InvisibilityScopeType}} seeInvisibleType, '''bool''' informExplorationTracking, '''bool''' alwaysSeeInvisible<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|change:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|seeInvisibleType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|informExplorationTracking:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alwaysSeeInvisible:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">pPlot:ChangeVisibilityCount(team, -1, -1, true, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">pPlot:ChangeVisibilityCount(team, 1, -1, true, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeVisibilityCount]]
[[Category:Civ5 Fog API|ChangeVisibilityCount]]
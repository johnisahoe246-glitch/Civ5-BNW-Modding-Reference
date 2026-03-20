{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.OnRecommendationCheckChanged<b>(</b>'''bool''' value<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.OnRecommendationCheckChanged.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.OnRecommendationCheckChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|value:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">LuaEvents.OnRecommendationCheckChanged.Add( SetRecommendationCheck );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">LuaEvents.OnRecommendationCheckChanged(mapOptions.HideTileRecommendations);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0411}}<syntaxhighlight lang="lua">LuaEvents.OnRecommendationCheckChanged( bIsChecked );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OnRecommendationCheckChanged]]
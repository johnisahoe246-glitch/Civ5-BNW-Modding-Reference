{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' StrategicViewShowFogOfWar<b>(</b>'''bool''' isChecked<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|isChecked:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">StrategicViewShowFogOfWar( mapOptions.SVShowFOW );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">StrategicViewShowFogOfWar( bIsChecked );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|StrategicViewShowFogOfWar]]
[[Category:Civ5 Fog API|StrategicViewShowFogOfWar]]
[[Category:Civ5 Diplomacy API|StrategicViewShowFogOfWar]]
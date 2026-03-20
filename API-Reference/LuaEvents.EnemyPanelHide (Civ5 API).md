{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.EnemyPanelHide<b>(</b>'''bool''' isHide<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.EnemyPanelHide.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.EnemyPanelHide(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|isHide:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1977}}<syntaxhighlight lang="lua">LuaEvents.EnemyPanelHide( bIsHide );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1381}}<syntaxhighlight lang="lua">LuaEvents.EnemyPanelHide.Add( OnEnemyPanelHide );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EnemyPanelHide]]
[[Category:Civ5 Diplomacy API|EnemyPanelHide]]
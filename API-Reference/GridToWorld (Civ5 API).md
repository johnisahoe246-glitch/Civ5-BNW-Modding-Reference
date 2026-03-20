{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''int''', '''int''', '''int''' GridToWorld<b>(</b>{{Type5|ResourceType}} gridX, '''int''' gridY<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|gridX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|gridY:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|PathHelpManager.lua}}
:<code>UI/InGame/WorldView/PathHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">local worldPosX, worldPosY, worldPosZ = GridToWorld( data.x, data.y );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0053}}<syntaxhighlight lang="lua">local x, y, z = GridToWorld( gridX, gridY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">local worldPosX, worldPosY, worldPosZ = GridToWorld( pUnit:GetX(), pUnit:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">local worldPos = Vector4( GridToWorld( pPlot:GetX(), pPlot:GetY() ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">local worldPosX, worldPosY, worldPosZ = GridToWorld( o.m_Unit:GetX(), o.m_Unit:GetY() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GridToWorld]]
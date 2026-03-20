{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' Game.CanHandleAction<b>(</b>{{Type5|ActionType}} action, {{Type5|Plot}} plot = nil, '''bool''' testVisible = false<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|action:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|testVisible:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">if(action.Visible and Game.CanHandleAction( iAction, 0, 1 ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">if( bShowActionButton and action.Visible and Game.CanHandleAction( iAction, 0, 1 ) )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">if not Game.CanHandleAction( iAction ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanHandleAction]]
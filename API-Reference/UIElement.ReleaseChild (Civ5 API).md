{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:ReleaseChild<b>(</b>{{Type5|WorldAnchor}} arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">Controls.ChatStack:ReleaseChild( g_ChatInstances[ 1 ].Box );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0040}}<syntaxhighlight lang="lua">Controls.NaturalWonderStore:ReleaseChild( instance.Anchor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">Controls.SettlerReccomendationStore:ReleaseChild( instance.Anchor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">Controls.WorkerReccomendationStore:ReleaseChild( instance.Anchor );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">Controls.SmallStack:ReleaseChild( instance[ name .. "Container" ] );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ReleaseChild]]
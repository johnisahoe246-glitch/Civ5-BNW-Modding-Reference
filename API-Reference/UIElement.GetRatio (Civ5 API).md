{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|ScrollPanel}} and {{Type5|Stack}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:GetRatio<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">if( Controls.MPListScroll:GetRatio() < 1 ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">if( Controls.SmallScrollPanel:GetRatio() ~= 1 ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetRatio]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''', '''int''' UIElement:GetOffsetVal<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local _, offsetY = Controls.OuterStack:GetOffsetVal();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetOffsetVal]]
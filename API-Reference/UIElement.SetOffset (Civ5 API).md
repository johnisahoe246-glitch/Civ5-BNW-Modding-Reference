{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetOffset<b>(</b>{{Type5|Vector2}} offset<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|offset:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0871}}<syntaxhighlight lang="lua">self.m_Instance.FlagShadow:SetOffset( offset );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetOffset]]
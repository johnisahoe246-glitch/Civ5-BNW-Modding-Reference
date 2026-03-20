{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetConsumeMouseOver<b>(</b>'''bool''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1595}}<syntaxhighlight lang="lua">pFlag.m_Instance.NormalButton:SetConsumeMouseOver( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1597}}<syntaxhighlight lang="lua">pFlag.m_Instance.HealthBarButton:SetConsumeMouseOver( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1600}}<syntaxhighlight lang="lua">pFlag.m_Instance.NormalButton:SetConsumeMouseOver( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1602}}<syntaxhighlight lang="lua">pFlag.m_Instance.HealthBarButton:SetConsumeMouseOver( false );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetConsumeMouseOver]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetOffsetY<b>(</b>'''int''' TOP_COMPENSATION<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|TOP_COMPENSATION:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0347}}<syntaxhighlight lang="lua">Controls.MPListScroll:SetOffsetY( TOP_COMPENSATION + CHAT_COMPENSATION );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0349}}<syntaxhighlight lang="lua">Controls.MPListScroll:SetOffsetY( TOP_COMPENSATION );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetOffsetY]]
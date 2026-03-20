{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''TextBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetWrapWidth<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TextPopup.lua}}
:<code>UI/InGame/Popups/TextPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">Controls.DescriptionLabel:SetWrapWidth( popupInfo.Data1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">Controls.DescriptionLabel:SetWrapWidth( 400 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetWrapWidth]]
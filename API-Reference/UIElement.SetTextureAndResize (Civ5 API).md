{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Image}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetTextureAndResize<b>(</b>'''string''' lastBackgroundImage<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|lastBackgroundImage:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">Controls.WonderSplash:SetTextureAndResize( thisBuilding.WonderSplashImage );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">Controls.WonderSplash:SetTextureAndResize( lastBackgroundImage );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetTextureAndResize]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.SetResourceVisibleMode<b>(</b>'''bool''' isChecked<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|isChecked:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">UI.SetResourceVisibleMode( mapOptions.ShowResources );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0364}}<syntaxhighlight lang="lua">UI.SetResourceVisibleMode(bIsChecked);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetResourceVisibleMode]]
[[Category:Civ5 Resources API|SetResourceVisibleMode]]
[[Category:Civ5 Fog API|SetResourceVisibleMode]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''', '''unknown''' Modding.GetDlcNameDescriptionKeys<b>(</b>'''int''' packageId<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|packageId:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">local dlcName, dlcDescription = Modding.GetDlcNameDescriptionKeys(packageId);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDlcNameDescriptionKeys]]
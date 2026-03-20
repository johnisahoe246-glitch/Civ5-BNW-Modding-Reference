{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Modding.AnyEnabledModsContainPropertyValue<b>(</b>'''string''' arg0, '''int''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ModsSinglePlayer.lua}}
:<code>UI/FrontEnd/Modding/ModsSinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">Controls.PlayMapButton:SetHide(Modding.AnyEnabledModsContainPropertyValue("HideSetupGame", 1));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AnyEnabledModsContainPropertyValue]]
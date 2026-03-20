{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Modding.GetModsRequiredToDisableMod<b>(</b>{{Type5|Button}} modID, {{Type5|Button}} version<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|modID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|version:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0347}}<syntaxhighlight lang="lua">local mods = Modding.GetModsRequiredToDisableMod(modID, version);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetModsRequiredToDisableMod]]
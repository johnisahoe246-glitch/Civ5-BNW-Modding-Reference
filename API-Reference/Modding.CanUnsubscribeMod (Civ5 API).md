{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' Modding.CanUnsubscribeMod<b>(</b>'''unknown''' modId, '''int''' modVersion<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|modId:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|modVersion:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0740}}<syntaxhighlight lang="lua">local bCanUnsubscribe = Modding.CanUnsubscribeMod(modId, modVersion);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0895}}<syntaxhighlight lang="lua">local bCanUnsubscribeMod = Modding.CanUnsubscribeMod(modId, version);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanUnsubscribeMod]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Modding.UpdateMod<b>(</b>{{Type5|Button}} arg0, {{Type5|Button}} arg1<b>)</b></code>


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
{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">updateBtn:RegisterCallback(Mouse.eLClick, function() Modding.UpdateMod(modinfo.ModId, modinfo.Version); end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UpdateMod]]
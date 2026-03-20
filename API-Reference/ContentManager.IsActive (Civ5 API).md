{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|ContentManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' ContentManager.IsActive<b>(</b>'''string''' v, {{Type5|ContentType}} arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|v:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua (G&K)}}
:<code>DLC/Expansion/UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0998}}<syntaxhighlight lang="lua">local bExpansionActive = ContentManager.IsActive("0E3751A1-F840-4e1b-9706-519BF484E59D", ContentType.GAMEPLAY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PremiumContentMenu.lua}}
:<code>UI/FrontEnd/PremiumContentMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">local bActive = ContentManager.IsActive(v, ContentType.GAMEPLAY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsActive]]
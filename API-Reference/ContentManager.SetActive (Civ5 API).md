{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|ContentManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' ContentManager.SetActive<b>(</b>table('''int''' => table('''int''' => '''string''')) packages<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|packages:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|PremiumContentMenu.lua}}
:<code>UI/FrontEnd/PremiumContentMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0044}}<syntaxhighlight lang="lua">ContentManager.SetActive(packages);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetActive]]
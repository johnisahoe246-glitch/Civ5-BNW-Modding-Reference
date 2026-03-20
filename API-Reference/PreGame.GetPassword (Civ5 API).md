{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' PreGame.GetPassword<b>(</b>'''int''' EditSlot<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|EditSlot:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0241}}<syntaxhighlight lang="lua">name = PreGame.GetPassword( g_EditSlot );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPassword]]
[[Category:Civ5 Game Settings API|GetPassword]]
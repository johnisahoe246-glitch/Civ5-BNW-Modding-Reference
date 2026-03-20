{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SetTurnSliceMaxMessageCount<b>(</b>'''int''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">Network.SetTurnSliceMaxMessageCount(Network.GetTurnSliceMaxMessageCount() - 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Network.SetTurnSliceMaxMessageCount(Network.GetTurnSliceMaxMessageCount() + 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetTurnSliceMaxMessageCount]]
[[Category:Civ5 Turns API|SetTurnSliceMaxMessageCount]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SetAdvisorMessageHasBeenSeen<b>(</b>'''unknown''' arg0, '''bool''' arg1<b>)</b></code>


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
{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">Game.SetAdvisorMessageHasBeenSeen(eventInfo.IDName, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetAdvisorMessageHasBeenSeen]]
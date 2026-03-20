{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendBarbarianRansom<b>(</b>'''int''' arg0, {{Type5|PlayerID}} unit<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|BarbarianRansomPopup.lua}}
:<code>UI/InGame/PopupsGeneric/BarbarianRansomPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">Network.SendBarbarianRansom(0, iUnitID);   -- 0 is Button ID</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">Network.SendBarbarianRansom(1, iUnitID);   -- 1 is Button ID</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendBarbarianRansom]]
[[Category:Civ5 Barbarians API|SendBarbarianRansom]]
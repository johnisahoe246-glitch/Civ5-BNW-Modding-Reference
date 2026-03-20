{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.LocationSelect<b>(</b>{{Type5|Plot}} plot, '''int''' ctrl, '''int''' alt, '''bool''' shift<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ctrl:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alt:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shift:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0125}}<syntaxhighlight lang="lua">UI.LocationSelect(plot, bCtrl, bAlt, bShift);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LocationSelect]]
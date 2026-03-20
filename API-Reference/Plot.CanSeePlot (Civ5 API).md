{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Plot:CanSeePlot<b>(</b>{{Type5|Plot}} target, {{Type5|TeamID}} team, '''int''' range<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|target:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|range:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">if not thisPlot:CanSeePlot(pTargetPlot, thisTeam, iRange - 1, NO_DIRECTION) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanSeePlot]]
[[Category:Civ5 Fog API|CanSeePlot]]
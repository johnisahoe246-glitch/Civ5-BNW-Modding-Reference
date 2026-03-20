{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:CanFound<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">if (bShow and not Players[Game.GetActivePlayer()]:CanFound(iPlotX, iPlotY)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanFound]]
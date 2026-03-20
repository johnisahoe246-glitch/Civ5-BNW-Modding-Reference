{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:CanEmbarkOnto<b>(</b>{{Type5|Plot}} plot, {{Type5|Plot}} targetPlot<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|targetPlot:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0445}}<syntaxhighlight lang="lua">return unit:CanEmbarkOnto(unit:GetPlot(), targetPlot);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">if (pHeadSelectedUnit:CanEmbarkOnto(pHeadSelectedUnit:GetPlot(), plot)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanEmbarkOnto]]
[[Category:Civ5 Movement API|CanEmbarkOnto]]
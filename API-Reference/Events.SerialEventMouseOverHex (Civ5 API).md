{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventMouseOverHex<b>(</b>'''int''' hexX, '''int''' hexY<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventMouseOverHex.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventMouseOverHex(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">Events.SerialEventMouseOverHex.Add( DisplayBombardArrow );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0238}}<syntaxhighlight lang="lua">Events.SerialEventMouseOverHex.Remove( DisplayBombardArrow );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0265}}<syntaxhighlight lang="lua">Events.SerialEventMouseOverHex.Add( DisplayNukeArrow );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">Events.SerialEventMouseOverHex.Remove( DisplayNukeArrow );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2149}}<syntaxhighlight lang="lua">Events.SerialEventMouseOverHex.Add( OnMouseOverHex );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">Events.SerialEventMouseOverHex.Add( DoUpdateXY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0749}}<syntaxhighlight lang="lua">Events.SerialEventMouseOverHex.Add( OnMouseMoveHex );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventMouseOverHex]]
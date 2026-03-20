{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SelectionListMove<b>(</b>{{Type5|Plot}} plot, '''int''' alt, '''bool''' shift, '''int''' ctrl<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alt:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shift:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ctrl:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvisorModal.lua}}
:<code>UI/InGame/Popups/AdvisorModal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">Game.SelectionListMove(g_referencePlot, false, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">Game.SelectionListMove(plot, false, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0663}}<syntaxhighlight lang="lua">Game.SelectionListMove(plot,  bAlt, bShift, bCtrl);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SelectionListMove]]
[[Category:Civ5 Movement API|SelectionListMove]]
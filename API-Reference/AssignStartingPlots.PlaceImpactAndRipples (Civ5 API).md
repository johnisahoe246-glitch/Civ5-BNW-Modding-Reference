{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:PlaceImpactAndRipples<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


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

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2738}}<syntaxhighlight lang="lua">self:PlaceImpactAndRipples(x, y)</syntaxhighlight>
{{CodeLine5|2739}}<syntaxhighlight lang="lua">return true, false</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2848}}<syntaxhighlight lang="lua">self:PlaceImpactAndRipples(best_fallback_x, best_fallback_y)</syntaxhighlight>
{{CodeLine5|2849}}<syntaxhighlight lang="lua">bSuccessFlag = true;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2860}}<syntaxhighlight lang="lua">self:PlaceImpactAndRipples(iWestX, iSouthY)</syntaxhighlight>
{{CodeLine5|2861}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlaceImpactAndRipples]]
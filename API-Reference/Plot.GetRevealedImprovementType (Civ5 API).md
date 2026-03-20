{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ImprovementType}} Plot:GetRevealedImprovementType<b>(</b>{{Type5|TeamID}} team, '''bool''' debug<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|debug:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">local iImprovementType = plot:GetRevealedImprovementType(iActiveTeam, bIsDebug);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetRevealedImprovementType]]
[[Category:Civ5 Improvements API|GetRevealedImprovementType]]
[[Category:Civ5 Fog API|GetRevealedImprovementType]]
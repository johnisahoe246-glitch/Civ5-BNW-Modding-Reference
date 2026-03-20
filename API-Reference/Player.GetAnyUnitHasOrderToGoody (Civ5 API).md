{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:GetAnyUnitHasOrderToGoody<b>(</b>'''unknown''' void<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|void:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0372}}<syntaxhighlight lang="lua">if (player:GetAnyUnitHasOrderToGoody()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetAnyUnitHasOrderToGoody]]
[[Category:Civ5 Goodies API|GetAnyUnitHasOrderToGoody]]
[[Category:Civ5 Units API|GetAnyUnitHasOrderToGoody]]
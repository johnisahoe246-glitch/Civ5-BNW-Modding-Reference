{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetFirstUnitOrder<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0643}}<syntaxhighlight lang="lua">if (v:GetFirstUnitOrder(GameInfo.Units.UNIT_WORKER.ID) ~= -1) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFirstUnitOrder]]
[[Category:Civ5 Units API|GetFirstUnitOrder]]
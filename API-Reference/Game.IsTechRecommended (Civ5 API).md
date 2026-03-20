{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' Game.IsTechRecommended<b>(</b>{{Type5|TechType}} arg0, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|advisorLoop:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0250}}<syntaxhighlight lang="lua">pControl:SetHide(not Game.IsTechRecommended(tech.ID, iAdvisorLoop));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsTechRecommended]]
[[Category:Civ5 Science API|IsTechRecommended]]
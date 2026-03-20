{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumResourceUsed<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">iUsed = pPlayer:GetNumResourceUsed( iResource );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">iNumUsed = pPlayer:GetNumResourceUsed(iResourceLoop);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResourceUsed]]
[[Category:Civ5 Resources API|GetNumResourceUsed]]
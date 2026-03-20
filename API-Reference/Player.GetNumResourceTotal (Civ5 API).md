{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumResourceTotal<b>(</b>{{Type5|ResourceType}} resource, '''bool''' includeImport<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|includeImport:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">if (pPlayer:GetNumResourceTotal(resourceID, true) > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0614}}<syntaxhighlight lang="lua">local iNum = pPlayer:GetNumResourceTotal(iResourceID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0740}}<syntaxhighlight lang="lua">local iNum = pPlayer:GetNumResourceTotal(iResourceID, false) + pPlayer:GetResourceExport(iResourceID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">iTotal = pPlayer:GetNumResourceTotal( iResource, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">iNumTotal = pPlayer:GetNumResourceTotal(iResourceLoop, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResourceTotal]]
[[Category:Civ5 Resources API|GetNumResourceTotal]]
[[Category:Civ5 Score API|GetNumResourceTotal]]
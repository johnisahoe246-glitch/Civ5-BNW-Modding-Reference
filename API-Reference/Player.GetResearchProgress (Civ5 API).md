{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetResearchProgress<b>(</b>{{Type5|TechType}} currentTech<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|currentTech:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TechHelpInclude.lua}}
:<code>UI/InGame/TechTree/TechHelpInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">local iProgress = pActivePlayer:GetResearchProgress(iTechID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">local iCurrentResearchProgress = pPlayer:GetResearchProgress(eCurrentTech);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0649}}<syntaxhighlight lang="lua">local currentResearchProgress = player:GetResearchProgress(techID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResearchProgress]]
[[Category:Civ5 Science API|GetResearchProgress]]
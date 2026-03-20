{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetResearchCost<b>(</b>{{Type5|TechType}} currentTech<b>)</b></code>


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
{{CodeLine5|0010}}<syntaxhighlight lang="lua">local iTechCost = pActivePlayer:GetResearchCost(iTechID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">local iResearchNeeded = pPlayer:GetResearchCost(eCurrentTech);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0650}}<syntaxhighlight lang="lua">local researchNeeded = player:GetResearchCost(techID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResearchCost]]
[[Category:Civ5 Science API|GetResearchCost]]
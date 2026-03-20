{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetResearchTurnsLeft<b>(</b>{{Type5|TechType}} tech, '''bool''' overflow<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tech:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|overflow:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">local iResearchTurnsLeft = pPlayer:GetResearchTurnsLeft(eCurrentTech, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0099}}<syntaxhighlight lang="lua">AddTechButton( tech, player:GetResearchTurnsLeft( techID, true ), iDiscover);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">local researchTurnsLeft = player:GetResearchTurnsLeft( tech.ID, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0175}}<syntaxhighlight lang="lua">local researchTurnsLeft = player:GetResearchTurnsLeft(techID, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">AddTechButton(tech, player:GetResearchTurnsLeft(techID, true), iDiscover);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0568}}<syntaxhighlight lang="lua">local researchTurnsLeft = player:GetResearchTurnsLeft( techID, true );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResearchTurnsLeft]]
[[Category:Civ5 Science API|GetResearchTurnsLeft]]
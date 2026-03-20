{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendResearch<b>(</b>{{Type5|PlayerID}} tech, {{Type5|ResourceType}} discover, '''int''' value, '''bool''' arg3 = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tech:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|discover:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|value:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0044}}<syntaxhighlight lang="lua">Network.SendResearch(eTech, iDiscover, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">Network.SendResearch(eTech, 0, iValue, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">Network.SendResearch(eTech, iValue, -1, false); -- iValue is number of free (non-espionage) techs</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">Network.SendResearch(eTech, player:GetNumFreeTechs(), -1, UIManager:GetShift());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua (G&K)}}
:<code>DLC/Expansion/UI/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">Network.SendResearch(eTech, 0, stealingTechTargetPlayerID, UIManager:GetShift());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendResearch]]
[[Category:Civ5 Science API|SendResearch]]
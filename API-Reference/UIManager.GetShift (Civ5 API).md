{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' UIManager.GetShift<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">local bShift = UIManager:GetShift();</syntaxhighlight>
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
[[Category:Civ5 Methods and Functions|GetShift]]
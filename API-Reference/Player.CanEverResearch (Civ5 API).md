{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:CanEverResearch<b>(</b>{{Type5|TechType}} tech<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tech:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0700}}<syntaxhighlight lang="lua">elseif (not player:CanEverResearch( techID ) or player:GetNumFreeTechs() > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua (G&K)}}
:<code>DLC/Expansion/UI/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0736}}<syntaxhighlight lang="lua">elseif (not player:CanEverResearch( techID ) or isAllowedToGetTechFree or stealingTechTargetPlayerID ~= -1) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanEverResearch]]
[[Category:Civ5 Science API|CanEverResearch]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ResourceType}} Player:GetNumFreeTechs<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">local iDiscover = player:GetNumFreeTechs();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">Network.SendResearch(eTech, player:GetNumFreeTechs(), -1, UIManager:GetShift());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0567}}<syntaxhighlight lang="lua">local numFreeTechs = player:GetNumFreeTechs();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0620}}<syntaxhighlight lang="lua">if player:GetNumFreeTechs() > 0 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0700}}<syntaxhighlight lang="lua">elseif (not player:CanEverResearch( techID ) or player:GetNumFreeTechs() > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua (G&K)}}
:<code>DLC/Expansion/UI/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0436}}<syntaxhighlight lang="lua">print("player:GetNumFreeTechs(): " ..  player:GetNumFreeTechs());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumFreeTechs]]
[[Category:Civ5 Science API|GetNumFreeTechs]]
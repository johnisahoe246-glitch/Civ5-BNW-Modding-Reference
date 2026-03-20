{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TechType}} Player:GetCurrentResearch<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">local currentTech = pOtherPlayer:GetCurrentResearch();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">eCurrentTech = pPlayer:GetCurrentResearch();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">local research = pPlayer:GetCurrentResearch();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">if player:GetCurrentResearch() == tech.ID then -- the player is currently researching this one</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0614}}<syntaxhighlight lang="lua">elseif player:GetCurrentResearch() == techID then -- the player is currently researching this one</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua (G&K)}}
:<code>DLC/Expansion/UI/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0650}}<syntaxhighlight lang="lua">elseif player:GetCurrentResearch() == techID and (not potentiallyBlockedFromStealing) then -- the player is currently researching this one</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2948}}<syntaxhighlight lang="lua">if (pPlayer:GetCurrentResearch() ~= -1) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCurrentResearch]]
[[Category:Civ5 Science API|GetCurrentResearch]]
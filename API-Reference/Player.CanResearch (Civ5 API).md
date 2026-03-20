{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CanResearch<b>(</b>{{Type5|TechType}} tech, '''bool''' trade = false<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tech:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|trade:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">if player:CanResearch( techID ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">elseif player:CanResearch( tech.ID ) then -- the player research this one right now if he wants</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0660}}<syntaxhighlight lang="lua">elseif (player:CanResearch( techID ) and not scienceDisabled) then -- the player research this one right now if he wants</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua (G&K)}}
:<code>DLC/Expansion/UI/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0696}}<syntaxhighlight lang="lua">elseif (player:CanResearch( techID ) and not scienceDisabled and (not potentiallyBlockedFromStealing)) then -- the player research this one right now if he wants</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanResearch]]
[[Category:Civ5 Science API|CanResearch]]
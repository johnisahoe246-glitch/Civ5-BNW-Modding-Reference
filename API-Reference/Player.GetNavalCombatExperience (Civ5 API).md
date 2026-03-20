{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNavalCombatExperience<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|GPList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">local fProgress  = pPlayer:GetNavalCombatExperience();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">fProgress  = pPlayer:GetNavalCombatExperience();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNavalCombatExperience]]
[[Category:Civ5 Unit Experience API|GetNavalCombatExperience]]
[[Category:Civ5 Combat API|GetNavalCombatExperience]]
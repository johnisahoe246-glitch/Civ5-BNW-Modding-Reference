{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetFoundedReligionFriendlyCityCombatMod<b>(</b>{{Type5|Plot}} toPlot<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|toPlot:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0895}}<syntaxhighlight lang="lua">iModifier = pMyPlayer:GetFoundedReligionFriendlyCityCombatMod(pToPlot);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1328}}<syntaxhighlight lang="lua">iModifier = pTheirPlayer:GetFoundedReligionFriendlyCityCombatMod(pToPlot);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1726}}<syntaxhighlight lang="lua">iModifier = pTheirPlayer:GetFoundedReligionFriendlyCityCombatMod(theirPlot);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFoundedReligionFriendlyCityCombatMod]]
[[Category:Civ5 Cities API|GetFoundedReligionFriendlyCityCombatMod]]
[[Category:Civ5 Religion API|GetFoundedReligionFriendlyCityCombatMod]]
[[Category:Civ5 Combat API|GetFoundedReligionFriendlyCityCombatMod]]
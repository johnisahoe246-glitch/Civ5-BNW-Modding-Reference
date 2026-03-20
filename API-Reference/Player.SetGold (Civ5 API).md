{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:SetGold<b>(</b>'''int''' newValue<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1610}}<syntaxhighlight lang="lua">pPlayer:SetGold(250)</syntaxhighlight>
{{CodeLine5|1611}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1626}}<syntaxhighlight lang="lua">pPlayer:SetGold(200)</syntaxhighlight>
{{CodeLine5|1627}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1636}}<syntaxhighlight lang="lua">pPlayer:SetGold(150)</syntaxhighlight>
{{CodeLine5|1637}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1646}}<syntaxhighlight lang="lua">pPlayer:SetGold(100)</syntaxhighlight>
{{CodeLine5|1647}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1653}}<syntaxhighlight lang="lua">pPlayer:SetGold(50)</syntaxhighlight>
{{CodeLine5|1654}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SWORDSMAN"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1660}}<syntaxhighlight lang="lua">pPlayer:SetGold(30)</syntaxhighlight>
{{CodeLine5|1661}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1684}}<syntaxhighlight lang="lua">pPlayer:SetGold(300)</syntaxhighlight>
{{CodeLine5|1685}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1703}}<syntaxhighlight lang="lua">pPlayer:SetGold(350)</syntaxhighlight>
{{CodeLine5|1704}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1728}}<syntaxhighlight lang="lua">pPlayer:SetGold(400)</syntaxhighlight>
{{CodeLine5|1729}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1756}}<syntaxhighlight lang="lua">pPlayer:SetGold(600)</syntaxhighlight>
{{CodeLine5|1757}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1787}}<syntaxhighlight lang="lua">pPlayer:SetGold(800)</syntaxhighlight>
{{CodeLine5|1788}}<syntaxhighlight lang="lua">iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetGold]]
[[Category:Civ5 Gold API|SetGold]]
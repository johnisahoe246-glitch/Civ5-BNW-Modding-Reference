{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''bool''' UnitMoving<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0966}}<syntaxhighlight lang="lua">if garrisonedUnit and not UnitMoving(garrisonedUnit:GetOwner(), garrisonedUnit:GetID()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1140}}<syntaxhighlight lang="lua">if bGarrisoned and not UnitMoving(playerID, unitID) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1115}}<syntaxhighlight lang="lua">if not UnitMoving(playerID, unitID) and g_MasterList[ playerID ] ~= nil then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitMoving]]
[[Category:Civ5 Units API|UnitMoving]]
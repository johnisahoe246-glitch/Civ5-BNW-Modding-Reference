{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|DB}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' DB.CreateQuery<b>(</b>'''string''' sql<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|sql:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0473}}<syntaxhighlight lang="lua">local UnitsByEra = DB.CreateQuery(sql);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0728}}<syntaxhighlight lang="lua">local BuildingsByEra = DB.CreateQuery(sql);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">local traitsQuery = DB.CreateQuery([[SELECT Description, ShortDescription FROM Traits inner join</syntaxhighlight>
{{CodeLine5|0153}}<syntaxhighlight lang="lua">Leader_Traits ON Traits.Type = Leader_Traits.TraitType</syntaxhighlight>
{{CodeLine5|0154}}<syntaxhighlight lang="lua">WHERE Leader_Traits.LeaderType = ? LIMIT 1]]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">local scenarioCivQuery = DB.CreateQuery(sql);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UniqueBonuses.lua}}
:<code>UI/FrontEnd/GameSetup/UniqueBonuses.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">local uniqueUnitsQuery = DB.CreateQuery([[SELECT ID, Description, PortraitIndex, IconAtlas from Units INNER JOIN</syntaxhighlight>
{{CodeLine5|0162}}<syntaxhighlight lang="lua">Civilization_UnitClassOverrides ON Units.Type = Civilization_UnitClassOverrides.UnitType</syntaxhighlight>
{{CodeLine5|0163}}<syntaxhighlight lang="lua">WHERE Civilization_UnitClassOverrides.CivilizationType = ? AND</syntaxhighlight>
{{CodeLine5|0164}}<syntaxhighlight lang="lua">Civilization_UnitClassOverrides.UnitType IS NOT NULL]]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0166}}<syntaxhighlight lang="lua">local uniqueBuildingsQuery = DB.CreateQuery([[SELECT ID, Description, PortraitIndex, IconAtlas from Buildings INNER JOIN</syntaxhighlight>
{{CodeLine5|0167}}<syntaxhighlight lang="lua">Civilization_BuildingClassOverrides ON Buildings.Type = Civilization_BuildingClassOverrides.BuildingType</syntaxhighlight>
{{CodeLine5|0168}}<syntaxhighlight lang="lua">WHERE Civilization_BuildingClassOverrides.CivilizationType = ? AND</syntaxhighlight>
{{CodeLine5|0169}}<syntaxhighlight lang="lua">Civilization_BuildingClassOverrides.BuildingType IS NOT NULL]]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">local uniqueImprovementsQuery = DB.CreateQuery([[SELECT ID, Description, PortraitIndex, IconAtlas from Improvements where CivilizationType = ?]]);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CreateQuery]]
[[Category:Civ5 City Production API|CreateQuery]]
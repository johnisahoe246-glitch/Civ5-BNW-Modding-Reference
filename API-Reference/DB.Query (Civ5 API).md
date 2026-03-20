{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|DB}}.<br/>
This is a static method, invoke it with a dot.
}}


Executes an arbitrary SQL statement on the gameplay database and returns recordset.
In situations where the quick and easy enumeration that ''GameInfo'' provides is not enough and either updates to the database or a complex query such as a join is required, DB.Query can be used.  This method executes any arbitrary SQL command on the gameplay database and returns a recordset.  Variable arguments can be used in the SQL command.  For information about how to use literal arguments, see [http://www.sqlite.org/c3ref/bind_blob.html| here].
The SQL command does not actually get executed until the query is iterated.  Even if your statement is not intended to return a record set, you must still iterate it to cause the "Step" to occur.


=Usage=
<code>'''string''' DB.Query<b>(</b>'''string''' SqlStatement, '''...''' statement_args = nil<b>)</b></code>


'''Returned Value'''
:A valid database query on success, nil on error.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|SqlStatement:
|valign="top"| ''A SQL string.''
|-
|valign="top" style="padding-right:6px;"|statement_args:
|valign="top"| ''One or many arguments that get injected into the SQL statement.
''Can be of type nil,number, or string.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
-- Obtain all custom map options which are dropdowns for the current map script and their possible values.
-- NOTE: Does not include checkbox-based options.
local sqlGetCustomMapOptions =
{{Type5|select * from MapScriptOptions
where
exists
(select 1 from MapScriptOptionPossibleValues
where
FileName = MapScriptOptions.FileName and
OptionID = MapScriptOptions.OptionID) and
Hidden = 0 and
FileName = ?}};
local currentMapScript = PreGame.GetMapScript();
for option in DB.Query(sqlGetCustomMapOptions, currentMapScript) do
options[option.OptionID] = {
ID = option.OptionID,
Name = Locale.ConvertTextKey(option.Name),
ToolTip = (option.Description) and Locale.ConvertTextKey(option.Description) or nil,
Disabled = (option.ReadOnly == 1) and true or false,
DefaultValue = option.DefaultValue,
SortPriority = option.SortPriority,
Values = {},
};
end</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">for option in DB.Query("select * from MapScriptOptions where exists (select 1 from MapScriptOptionPossibleValues where FileName = MapScriptOptions.FileName and OptionID = MapScriptOptions.OptionID) and Hidden = 0 and FileName = ?", currentMapScript) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">for possibleValue in DB.Query("select * from MapScriptOptionPossibleValues where FileName = ? order by SortIndex ASC", currentMapScript) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">for option in DB.Query("select * from MapScriptOptions where not exists (select 1 from MapScriptOptionPossibleValues where FileName = MapScriptOptions.FileName and OptionID = MapScriptOptions.OptionID) and Hidden = 0 and FileName = ?", PreGame.GetMapScript()) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">for row in DB.Query(sql) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1370}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Technologies ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1403}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Units ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1435}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from UnitPromotions ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1467}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Buildings where WonderSplashImage IS NULL ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1499}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Buildings Where WonderSplashImage IS NOT NULL ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1531}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Policies Where IconAtlas IS NOT NULL ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1587}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Leaders where Type <> \"LEADER_BARBARIAN\" ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1645}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Terrains ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1683}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Resources ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1716}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Improvements ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0460}}<syntaxhighlight lang="lua">for unit in DB.Query("SELECT Units.ID, Units.Description, Units.PortraitIndex, Units.IconAtlas From Units where FaithCost > 0 and not RequiresFaithPurchaseEnabled and ShowInPedia == 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0489}}<syntaxhighlight lang="lua">for unit in DB.Query("SELECT Units.ID, Units.Description, Units.PortraitIndex, Units.IconAtlas From Units where PreReqTech is NULL and Special is NULL and (Units.FaithCost = 0 or RequiresFaithPurchaseEnabled) and Units.ShowInPedia = 1") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0714}}<syntaxhighlight lang="lua">for building in DB.Query("SELECT Buildings.ID, Buildings.Description, Buildings.PortraitIndex, Buildings.IconAtlas from Buildings inner join  BuildingClasses on Buildings.BuildingClass = BuildingClasses.Type where FaithCost > 0 and BuildingClasses.MaxGlobalInstances < 0 and BuildingClasses.MaxPlayerInstances <> 1 and BuildingClasses.MaxTeamInstances < 0;") do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0752}}<syntaxhighlight lang="lua">for building in DB.Query(sql) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1588}}<syntaxhighlight lang="lua">for row in DB.Query("SELECT PortraitIndex, IconAtlas from Policies ORDER By Random() LIMIT 1") do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameCalendarUtilities.lua}}
:<code>Gameplay/Lua/GameCalendarUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">for row in DB.Query([[SELECT MonthIncrement, TurnsPerIncrement FROM GameSpeed_Turns WHERE GameSpeedType = ? ORDER BY rowid ASC]], gameSpeedType) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapmakerUtilities.lua}}
:<code>Gameplay/Lua/MapmakerUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0466}}<syntaxhighlight lang="lua">for row in DB.Query("select count(*) as count from Civilization_Start_Region_Priority where CivilizationType = ?", civType) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0474}}<syntaxhighlight lang="lua">for row in DB.Query("select count(*) as count from Civilization_Start_Region_Avoid where CivilizationType = ?", civType) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1019}}<syntaxhighlight lang="lua">for row in DB.Query([[SELECT</syntaxhighlight>
{{CodeLine5|1020}}<syntaxhighlight lang="lua">   Civilizations.ID as CivID,</syntaxhighlight>
{{CodeLine5|1021}}<syntaxhighlight lang="lua">   Civilizations.Description as CivDescription,</syntaxhighlight>
{{CodeLine5|1022}}<syntaxhighlight lang="lua">   Civilizations.ShortDescription as CivShortDescription,</syntaxhighlight>
{{CodeLine5|1023}}<syntaxhighlight lang="lua">   Leaders.Description as LeaderDescription</syntaxhighlight>
{{CodeLine5|1024}}<syntaxhighlight lang="lua">   FROM Civilizations, Leaders, Civilization_Leaders</syntaxhighlight>
{{CodeLine5|1025}}<syntaxhighlight lang="lua">   WHERE</syntaxhighlight>
{{CodeLine5|1026}}<syntaxhighlight lang="lua">   Civilizations.Playable = 1 AND</syntaxhighlight>
{{CodeLine5|1027}}<syntaxhighlight lang="lua">   Civilizations.Type = Civilization_Leaders.CivilizationType AND</syntaxhighlight>
{{CodeLine5|1028}}<syntaxhighlight lang="lua">   Leaders.Type = Civilization_Leaders.LeaderheadType</syntaxhighlight>
{{CodeLine5|1029}}<syntaxhighlight lang="lua">   ]]) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UniqueBonuses.lua}}
:<code>UI/FrontEnd/GameSetup/UniqueBonuses.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">for row in DB.Query([[SELECT ID, Description, PortraitIndex, IconAtlas from Units INNER JOIN</syntaxhighlight>
{{CodeLine5|0113}}<syntaxhighlight lang="lua">   Civilization_UnitClassOverrides ON Units.Type = Civilization_UnitClassOverrides.UnitType</syntaxhighlight>
{{CodeLine5|0114}}<syntaxhighlight lang="lua">   WHERE Civilization_UnitClassOverrides.CivilizationType = ? AND</syntaxhighlight>
{{CodeLine5|0115}}<syntaxhighlight lang="lua">   Civilization_UnitClassOverrides.UnitType IS NOT NULL]], civ.Type) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">for row in DB.Query([[SELECT ID, Description, PortraitIndex, IconAtlas from Buildings INNER JOIN</syntaxhighlight>
{{CodeLine5|0121}}<syntaxhighlight lang="lua">   Civilization_BuildingClassOverrides ON Buildings.Type = Civilization_BuildingClassOverrides.BuildingType</syntaxhighlight>
{{CodeLine5|0122}}<syntaxhighlight lang="lua">   WHERE Civilization_BuildingClassOverrides.CivilizationType = ? AND</syntaxhighlight>
{{CodeLine5|0123}}<syntaxhighlight lang="lua">   Civilization_BuildingClassOverrides.BuildingType IS NOT NULL]], civ.Type) do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">for row in DB.Query([[SELECT ID, Description, PortraitIndex, IconAtlas from Improvements where CivilizationType = ?]], civ.Type) do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Query]]
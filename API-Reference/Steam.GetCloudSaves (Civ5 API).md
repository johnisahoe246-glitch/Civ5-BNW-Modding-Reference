{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Obtains information about all Steam Cloud saved games


=Usage=
<code>table({{Type5|SpecialistType}} => {{Type5|FileHeader}}) Steam.GetCloudSaves<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns an list of tables where each table is information about a specific save.
:The table is indexed by the save slot number.
:NOTE: Empty save slots are nil in the table and thus you should not iterate using ipairs.
:Each save in the list has the following fields:
::PlayerCivilization - ''The current player's Civilizations type.
::GameSpeed - ''The GameSpeeds type.
::StartEra - ''The starting Eras type.
::CurrentEra - ''The current Eras type.
::TurnNumber - ''The current turn number.
::Difficulty - ''The HandicapInfos type currently in use.
::WorldSize - ''The Worlds type currently in use.
::MapScript- ''The name of the map script or Worldbuilder map used.
::CivilizationName - ''The user-supplied Civilization Name.
::LeaderName - ''The user-supplied Leader Name.
::PlayerColor - ''The PlayerColor Type.
::ActivatedMods - ''This is an array of tables.
:Each activated mod entry has the following fields:
:ModID - ''The GUID of the Mod.
:Version - ''The Version of the Mod.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
for i, save in pairs(Steam.GetCloudSaves()) do
local civ_description = GameInfo.Civilizations[saves.PlayerCivilization].Description;
local localized_civ = Locale.ConvertTextKey(civ_description);
print(string.format("Slot %i: %s - Turn %i", i, localized_civ, save.TurnNumber));
end</syntaxhighlight>


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0707}}<syntaxhighlight lang="lua">g_CloudSaves = Steam.GetCloudSaves();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0502}}<syntaxhighlight lang="lua">local cloudSaveData = Steam.GetCloudSaves();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCloudSaves]]
{|align="right"
|[[Civ4 XML Reference|Back to XML Reference]]
|}<br>
== Do not edit schema files unless you know EXACTLY what you are doing!!! ==
Civ IV uses the DLL (editable through the SDK) to read the Schema files, and then uses the Schema data to parse the XML. Messing with the Schema and not making appropriate changes to the SDK can result in the game crashing.  Any changes to the Schema '''''must''''' be reflected in the SDK.  Removing schema entries without changing the DLL appropriately '''''will''''' result in a crash, while adding entries without editing the SDK will simply cause nothing to happen.  Changes to the schema files also must be reflected in the XML files they are used for.

== Schema Table ==
This table lists the files affected by each schema file.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Schema File
! style="background:#efefef;" | Files Affected
|-
! Civ4GlobalDefinesSchema
| Most files in Assets\XML (but not subfolders)
|-
! Civ4GlobalTypesSchema
| GlobalTypes.xml
|-
! Civ4ArtDefinesSchema
| All files in XML\Art
|-
! AudioDefinesSchema
| AudioDefines.xml
|-
! AudioScriptSchema
| Most files in XML\Audio
|-
! Civ4BasicInfoSchema
| All files in XML\BasicInfos
|-
! Civ4BuildingsSchema
| Most files in XML\Buildings
|-
! Civ4LSystemSchema
| Civ4CityLSystem.xml, Civ4PlotLSystem.xml
|-
! Civ4CivilizationsSchema
| All files in XML\Civilizations
|-
! Civ4EventSchema
| All files in XML\Events
|-
! Civ4GameInfoSchema
| All files in XML\GameInfo
|-
! Civ4InterfaceSchema
| All files in XML\Interface
|-
! Civ4DetailManagerSchema
| Civ4DetailManager.xml
|-
! Civ4MiscSchema
| Most files in XML\Misc
|-
! Civ4TutorialSchema
| Civ4TutorialInfos.xml
|-
! Civ4TechnologiesSchema
| All files in XML\Technologies
|-
! Civ4TerrainSchema
| All files in XML\Terrain
|-
! Civ4FormationSchema
| Civ4FormationInfos.xml
|-
! Civ4UnitSchema
| Most files in XML\Units
|}
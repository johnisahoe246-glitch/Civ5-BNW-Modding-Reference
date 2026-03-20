{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>UnitType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>UnitType</code> corresponds to the ''ID'' column of the {{Table5|Units|CIV5Units}} XML table.
}}


= XML: the Units table =
Here are the ''ID'' and ''Type'' columns found in this table.
<code>
{|
|-
!align="left" |ID
!
!align="left" |Type
|-
|align="right"|0
|
|UNIT_SETTLER
|-
|align="right"|0
|
|UNIT_PROPHET
|-
|align="right"|1
|
|UNIT_WORKER
|-
|align="right"|1
|
|UNIT_CELT_PICTISH_WARRIOR
|-
|align="right"|2
|
|UNIT_WORKBOAT
|-
|align="right"|2
|
|UNIT_MAYAN_ATLATLIST
|-
|align="right"|3
|
|UNIT_ARTIST
|-
|align="right"|3
|
|UNIT_BYZANTINE_DROMON
|-
|align="right"|4
|
|UNIT_SCIENTIST
|-
|align="right"|4
|
|UNIT_BYZANTINE_CATAPHRACT
|-
|align="right"|5
|
|UNIT_MERCHANT
|-
|align="right"|5
|
|UNIT_CARTHAGINIAN_FOREST_ELEPHANT
|-
|align="right"|6
|
|UNIT_ENGINEER
|-
|align="right"|6
|
|UNIT_CARTHAGINIAN_QUINQUEREME
|-
|align="right"|7
|
|UNIT_GREAT_GENERAL
|-
|align="right"|7
|
|UNIT_HUN_HORSE_ARCHER
|-
|align="right"|8
|
|UNIT_SS_STASIS_CHAMBER
|-
|align="right"|8
|
|UNIT_AUSTRIAN_HUSSAR
|-
|align="right"|9
|
|UNIT_SS_ENGINE
|-
|align="right"|9
|
|UNIT_ETHIOPIAN_MEHAL_SEFARI
|-
|align="right"|10
|
|UNIT_SS_COCKPIT
|-
|align="right"|10
|
|UNIT_MISSIONARY
|-
|align="right"|11
|
|UNIT_SS_BOOSTER
|-
|align="right"|11
|
|UNIT_COMPOSITE_BOWMAN
|-
|align="right"|12
|
|UNIT_MISSILE_CRUISER
|-
|align="right"|12
|
|UNIT_GALLEASS
|-
|align="right"|13
|
|UNIT_NUCLEAR_SUBMARINE
|-
|align="right"|13
|
|UNIT_GREAT_WAR_INFANTRY
|-
|align="right"|14
|
|UNIT_CARRIER
|-
|align="right"|14
|
|UNIT_MARINE
|-
|align="right"|15
|
|UNIT_BATTLESHIP
|-
|align="right"|15
|
|UNIT_TRIPLANE
|-
|align="right"|16
|
|UNIT_SUBMARINE
|-
|align="right"|16
|
|UNIT_WWI_BOMBER
|-
|align="right"|17
|
|UNIT_DESTROYER
|-
|align="right"|17
|
|UNIT_WWI_TANK
|-
|align="right"|18
|
|UNIT_IRONCLAD
|-
|align="right"|18
|
|UNIT_MACHINE_GUN
|-
|align="right"|19
|
|UNIT_FRIGATE
|-
|align="right"|19
|
|UNIT_SWEDISH_CAROLEAN
|-
|align="right"|20
|
|UNIT_ENGLISH_SHIPOFTHELINE
|-
|align="right"|20
|
|UNIT_SWEDISH_HAKKAPELIITTA
|-
|align="right"|21
|
|UNIT_CARAVEL
|-
|align="right"|21
|
|UNIT_HUN_BATTERING_RAM
|-
|align="right"|22
|
|UNIT_TRIREME
|-
|align="right"|22
|
|UNIT_PRIVATEER
|-
|align="right"|23
|
|UNIT_MECH
|-
|align="right"|23
|
|UNIT_DUTCH_SEA_BEGGAR
|-
|align="right"|24
|
|UNIT_NUCLEAR_MISSILE
|-
|align="right"|24
|
|UNIT_INQUISITOR
|-
|align="right"|25
|
|UNIT_STEALTH_BOMBER
|-
|align="right"|25
|
|UNIT_GREAT_ADMIRAL
|-
|align="right"|26
|
|UNIT_JET_FIGHTER
|-
|align="right"|26
|
|UNIT_GATLINGGUN
|-
|align="right"|27
|
|UNIT_GUIDED_MISSILE
|-
|align="right"|28
|
|UNIT_MODERN_ARMOR
|-
|align="right"|29
|
|UNIT_HELICOPTER_GUNSHIP
|-
|align="right"|30
|
|UNIT_MOBILE_SAM
|-
|align="right"|31
|
|UNIT_ROCKET_ARTILLERY
|-
|align="right"|32
|
|UNIT_MECHANIZED_INFANTRY
|-
|align="right"|33
|
|UNIT_ATOMIC_BOMB
|-
|align="right"|34
|
|UNIT_BOMBER
|-
|align="right"|35
|
|UNIT_AMERICAN_B17
|-
|align="right"|36
|
|UNIT_FIGHTER
|-
|align="right"|37
|
|UNIT_JAPANESE_ZERO
|-
|align="right"|38
|
|UNIT_PARATROOPER
|-
|align="right"|39
|
|UNIT_TANK
|-
|align="right"|40
|
|UNIT_GERMAN_PANZER
|-
|align="right"|41
|
|UNIT_ARTILLERY
|-
|align="right"|42
|
|UNIT_ANTI_AIRCRAFT_GUN
|-
|align="right"|43
|
|UNIT_ANTI_TANK_GUN
|-
|align="right"|44
|
|UNIT_INFANTRY
|-
|align="right"|45
|
|UNIT_FRENCH_FOREIGNLEGION
|-
|align="right"|46
|
|UNIT_CAVALRY
|-
|align="right"|47
|
|UNIT_RUSSIAN_COSSACK
|-
|align="right"|48
|
|UNIT_RIFLEMAN
|-
|align="right"|49
|
|UNIT_LANCER
|-
|align="right"|50
|
|UNIT_OTTOMAN_SIPAHI
|-
|align="right"|51
|
|UNIT_CANNON
|-
|align="right"|52
|
|UNIT_MUSKETMAN
|-
|align="right"|53
|
|UNIT_AMERICAN_MINUTEMAN
|-
|align="right"|54
|
|UNIT_FRENCH_MUSKETEER
|-
|align="right"|55
|
|UNIT_OTTOMAN_JANISSARY
|-
|align="right"|56
|
|UNIT_LONGSWORDSMAN
|-
|align="right"|57
|
|UNIT_JAPANESE_SAMURAI
|-
|align="right"|58
|
|UNIT_TREBUCHET
|-
|align="right"|59
|
|UNIT_KNIGHT
|-
|align="right"|60
|
|UNIT_ARABIAN_CAMELARCHER
|-
|align="right"|61
|
|UNIT_SIAMESE_WARELEPHANT
|-
|align="right"|62
|
|UNIT_SONGHAI_MUSLIMCAVALRY
|-
|align="right"|63
|
|UNIT_CROSSBOWMAN
|-
|align="right"|64
|
|UNIT_CHINESE_CHUKONU
|-
|align="right"|65
|
|UNIT_ENGLISH_LONGBOWMAN
|-
|align="right"|66
|
|UNIT_PIKEMAN
|-
|align="right"|67
|
|UNIT_GERMAN_LANDSKNECHT
|-
|align="right"|68
|
|UNIT_CATAPULT
|-
|align="right"|69
|
|UNIT_ROMAN_BALLISTA
|-
|align="right"|70
|
|UNIT_HORSEMAN
|-
|align="right"|71
|
|UNIT_GREEK_COMPANIONCAVALRY
|-
|align="right"|72
|
|UNIT_SWORDSMAN
|-
|align="right"|73
|
|UNIT_IROQUOIAN_MOHAWKWARRIOR
|-
|align="right"|74
|
|UNIT_ROMAN_LEGION
|-
|align="right"|75
|
|UNIT_CHARIOT_ARCHER
|-
|align="right"|76
|
|UNIT_EGYPTIAN_WARCHARIOT
|-
|align="right"|77
|
|UNIT_INDIAN_WARELEPHANT
|-
|align="right"|78
|
|UNIT_SPEARMAN
|-
|align="right"|79
|
|UNIT_GREEK_HOPLITE
|-
|align="right"|80
|
|UNIT_PERSIAN_IMMORTAL
|-
|align="right"|81
|
|UNIT_ARCHER
|-
|align="right"|82
|
|UNIT_SCOUT
|-
|align="right"|83
|
|UNIT_WARRIOR
|-
|align="right"|84
|
|UNIT_AZTEC_JAGUAR
|-
|align="right"|85
|
|UNIT_BARBARIAN_WARRIOR
|-
|align="right"|86
|
|UNIT_GALLEY
|-
|align="right"|87
|
|UNIT_BARBARIAN_ARCHER
|-
|align="right"|88
|
|UNIT_BARBARIAN_SPEARMAN
|-
|align="right"|89
|
|UNIT_BARBARIAN_SWORDSMAN
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Units.UNIT_PROPHET.ID
local id = GameInfo["Units"].["UNIT_PROPHET"].ID
local id = GameInfo.Units{Type="UNIT_PROPHET"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_UNIT_GREAT_PROPHET.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Units[0].Description
local description = GameInfo["Units"][0]["Description"]
local description = GameInfo.Units{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETHELPTEXTFORUNIT
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetHelpTextForUnit}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' includeRequirementsInfo<b>)</b></code>
<!-- 
ALLUPGRADESAVAILABLE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|AllUpgradesAvailable}}<b>(</b>{{Type5|UnitType}} unit, '''int''' upgradeCount = 0<b>)</b></code>
<!-- 
CANTRAIN
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanTrain}}<b>(</b>{{Type5|UnitType}} unit, '''int''' continue, '''int''' testVisible, '''bool''' ignoreCost, '''bool''' ignoreUpgrades<b>)</b></code>
<!-- 
CANTRAINTOOLTIP
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanTrainTooltip}}<b>(</b>{{Type5|UnitType}} id<b>)</b></code>
<!-- 
CHANGEGREATPEOPLEUNITPROGRESS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChangeGreatPeopleUnitProgress}}<b>(</b>{{Type5|UnitType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEUNITPRODUCTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChangeUnitProduction}}<b>(</b>{{Type5|UnitType}} index, '''int''' change<b>)</b></code>
<!-- 
CHOOSEPRODUCTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChooseProduction}}<b>(</b>{{Type5|UnitType}} trainUnit, {{Type5|BuildingType}} constructBuilding, {{Type5|ProjectType}} createProject, '''bool''' finish, '''bool''' front<b>)</b></code>
<!-- 
CREATEGREATGENERAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CreateGreatGeneral}}<b>(</b>{{Type5|UnitType}} greatPersonUnit<b>)</b></code>
<!-- 
GETCONSCRIPTUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetConscriptUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHPURCHASEUNITTOOLTIP
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetFaithPurchaseUnitTooltip}}<b>(</b>{{Type5|UnitType}} id<b>)</b></code>
<!-- 
GETFIRSTUNITORDER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetFirstUnitOrder}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETGREATPEOPLEUNITPROGRESS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetGreatPeopleUnitProgress}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
GETGREATPEOPLEUNITRATE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetGreatPeopleUnitRate}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
GETPRODUCTIONEXPERIENCE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProductionExperience}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETPRODUCTIONUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProductionUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPURCHASEUNITTOOLTIP
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetPurchaseUnitTooltip}}<b>(</b>{{Type5|UnitType}} id<b>)</b></code>
<!-- 
GETUNITFAITHPURCHASECOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetUnitFaithPurchaseCost}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' arg1<b>)</b></code>
<!-- 
GETUNITPRODUCTIONMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetUnitProductionModifier}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETUNITPRODUCTIONTURNSLEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetUnitProductionTurnsLeft}}<b>(</b>{{Type5|UnitType}} unit, '''int''' num<b>)</b></code>
<!-- 
GETUNITPURCHASECOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetUnitPurchaseCost}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
ISCANPURCHASE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsCanPurchase}}<b>(</b>{{Type5|UnitType}} unitType, '''int''' buildingType, '''int''' projectType, '''int''' projectID, '''int''' projectID = nil, {{Type5|YieldType}} yield = nil<b>)</b></code>
<!-- 
ISUNITFOODPRODUCTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsUnitFoodProduction}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
SETGREATPEOPLEUNITPROGRESS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetGreatPeopleUnitProgress}}<b>(</b>{{Type5|UnitType}} index, '''int''' newValue<b>)</b></code>
<!-- 
CITYPURCHASEBUILDING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseBuilding}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEPROJECT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseProject}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseUnit}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPUSHORDER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPushOrder}}<b>(</b>{{Type5|City}} city, {{Type5|OrderType}} order, {{Type5|UnitType}} data, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
GETBESTLANDUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBestLandUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBESTLANDUNITCOMBAT
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBestLandUnitCombat}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFAITHCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetFaithCost}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETNUMRESOURCEREQUIREDFORUNIT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetNumResourceRequiredForUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETUNITCREATEDCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetUnitCreatedCount}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
GETUNITUPGRADESTO
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetUnitUpgradesTo}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
ISUNITEVERACTIVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsUnitEverActive}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
<!-- 
ADDFREEUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|AddFreeUnit}}<b>(</b>{{Type5|UnitType}} arg0, {{Type5|UnitAIType}} UNITAI_DEFENSE<b>)</b></code>
<!-- 
CANTRAIN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanTrain}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' continue, '''bool''' testVisible, '''bool''' arg3, '''bool''' arg4<b>)</b></code>
<!-- 
DOGREATPERSONCHOICE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoGreatPersonChoice}}<b>(</b>'''int''' cityID, '''bool''' spawnUnit, {{Type5|UnitType}} unit<b>)</b></code>
<!-- 
GETADVANCEDSTARTUNITCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartUnitCost}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' add, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETMINORCIVUNIQUEUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivUniqueUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUNITBAKTUN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnitBaktun}}<b>(</b>{{Type5|UnitType}} arg0<b>)</b></code>
<!-- 
GETUNITPRODUCTIONNEEDED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetUnitProductionNeeded}}<b>(</b>{{Type5|UnitType}} index<b>)</b></code>
<!-- 
INITUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|InitUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|UnitAIType}} unitAI = NO_UNITAI, {{Type5|DirectionType}} facingDirection = NO_DIRECTION<b>)</b></code>
<!-- 
ISCANPURCHASEANYCITY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsCanPurchaseAnyCity}}<b>(</b>'''bool''' arg0, '''bool''' arg1, {{Type5|UnitType}} arg2, {{Type5|BuildingType}} arg3, {{Type5|YieldType}} arg4<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TextButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} OnSearchTextEnter, ('''void''' func<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex, {{Type5|UnitType}} y, {{Type5|Button}} button<b>)</b>) OnClose = nil<b>)</b></code>
<!-- 
GETINTERFACEMODEDEBUGITEMID2
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetInterfaceModeDebugItemID2}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAPPLAYERS
-->
|-
|align="right" width="200" |<code>table({{Type5|UnitType}} => '''Civilizations.row''')</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetMapPlayers}}<b>(</b>'''string''' mapScriptPath<b>)</b></code>
<!-- 
MOVESCENARIOPLAYERTOSLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|MoveScenarioPlayerToSlot}}<b>(</b>{{Type5|UnitType}} playerIndex, '''int''' arg1<b>)</b></code>
<!-- 
GETCAPTUREUNITTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetCaptureUnitType}}<b>(</b>{{Type5|CivilizationType}} civilization<b>)</b></code>
<!-- 
GETUNITTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUnitType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETUPGRADEUNITTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUpgradeUnitType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHIGHERTECHTHAN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsHigherTechThan}}<b>(</b>{{Type5|UnitType}} arg0<b>)</b></code>
<!-- 
SETLEADERUNITTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|SetLeaderUnitType}}<b>(</b>{{Type5|UnitType}} leaderUnitType<b>)</b></code>
<!-- 
UPGRADEPRICE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|UpgradePrice}}<b>(</b>{{Type5|UnitType}} unit<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|UnitType]]
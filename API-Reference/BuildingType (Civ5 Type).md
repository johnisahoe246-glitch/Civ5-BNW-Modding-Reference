{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>BuildingType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>BuildingType</code> corresponds to the ''ID'' column of the {{Table5|Buildings|CIV5Buildings}} XML table.
}}


= XML: the Buildings table =
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
|BUILDING_COURTHOUSE
|-
|align="right"|0
|
|BUILDING_FLOATING_GARDENS
|-
|align="right"|0
|
|BUILDING_AMPHITHEATER
|-
|align="right"|1
|
|BUILDING_MUGHAL_FORT
|-
|align="right"|1
|
|BUILDING_SHRINE
|-
|align="right"|2
|
|BUILDING_KREPOST
|-
|align="right"|2
|
|BUILDING_RECYCLING_CENTER
|-
|align="right"|3
|
|BUILDING_LONGHOUSE
|-
|align="right"|3
|
|BUILDING_BOMB_SHELTER
|-
|align="right"|4
|
|BUILDING_BAZAAR
|-
|align="right"|4
|
|BUILDING_CONSTABLE
|-
|align="right"|5
|
|BUILDING_SATRAPS_COURT
|-
|align="right"|5
|
|BUILDING_POLICE_STATION
|-
|align="right"|6
|
|BUILDING_PAPER_MAKER
|-
|align="right"|6
|
|BUILDING_INTELLIGENCE_AGENCY
|-
|align="right"|7
|
|BUILDING_WAT
|-
|align="right"|7
|
|BUILDING_ALHAMBRA
|-
|align="right"|8
|
|BUILDING_MUD_PYRAMID_MOSQUE
|-
|align="right"|8
|
|BUILDING_CN_TOWER
|-
|align="right"|9
|
|BUILDING_BURIAL_TOMB
|-
|align="right"|9
|
|BUILDING_HUBBLE
|-
|align="right"|10
|
|BUILDING_SEAPORT
|-
|align="right"|10
|
|BUILDING_LEANING_TOWER
|-
|align="right"|11
|
|BUILDING_STABLE
|-
|align="right"|11
|
|BUILDING_MOSQUE_OF_DJENNE
|-
|align="right"|12
|
|BUILDING_WATERMILL
|-
|align="right"|12
|
|BUILDING_NEUSCHWANSTEIN
|-
|align="right"|13
|
|BUILDING_CIRCUS
|-
|align="right"|13
|
|BUILDING_PETRA
|-
|align="right"|14
|
|BUILDING_FORGE
|-
|align="right"|14
|
|BUILDING_TERRACOTTA_ARMY
|-
|align="right"|15
|
|BUILDING_WINDMILL
|-
|align="right"|15
|
|BUILDING_GREAT_FIREWALL
|-
|align="right"|16
|
|BUILDING_HYDRO_PLANT
|-
|align="right"|16
|
|BUILDING_CATHEDRAL
|-
|align="right"|17
|
|BUILDING_SOLAR_PLANT
|-
|align="right"|17
|
|BUILDING_MOSQUE
|-
|align="right"|18
|
|BUILDING_MINT
|-
|align="right"|18
|
|BUILDING_PAGODA
|-
|align="right"|19
|
|BUILDING_OBSERVATORY
|-
|align="right"|19
|
|BUILDING_CEILIDH_HALL
|-
|align="right"|20
|
|BUILDING_MONASTERY
|-
|align="right"|20
|
|BUILDING_COFFEE_HOUSE
|-
|align="right"|21
|
|BUILDING_GARDEN
|-
|align="right"|21
|
|BUILDING_STELE
|-
|align="right"|22
|
|BUILDING_LIGHTHOUSE
|-
|align="right"|22
|
|BUILDING_MAYA_PYRAMID
|-
|align="right"|23
|
|BUILDING_HARBOR
|-
|align="right"|24
|
|BUILDING_COLOSSEUM
|-
|align="right"|25
|
|BUILDING_THEATRE
|-
|align="right"|26
|
|BUILDING_STADIUM
|-
|align="right"|27
|
|BUILDING_MONUMENT
|-
|align="right"|28
|
|BUILDING_TEMPLE
|-
|align="right"|29
|
|BUILDING_OPERA_HOUSE
|-
|align="right"|30
|
|BUILDING_MUSEUM
|-
|align="right"|31
|
|BUILDING_BROADCAST_TOWER
|-
|align="right"|32
|
|BUILDING_BARRACKS
|-
|align="right"|33
|
|BUILDING_ARMORY
|-
|align="right"|34
|
|BUILDING_MILITARY_ACADEMY
|-
|align="right"|35
|
|BUILDING_ARSENAL
|-
|align="right"|36
|
|BUILDING_WALLS
|-
|align="right"|37
|
|BUILDING_CASTLE
|-
|align="right"|38
|
|BUILDING_MILITARY_BASE
|-
|align="right"|39
|
|BUILDING_GRANARY
|-
|align="right"|40
|
|BUILDING_HOSPITAL
|-
|align="right"|41
|
|BUILDING_MEDICAL_LAB
|-
|align="right"|42
|
|BUILDING_WORKSHOP
|-
|align="right"|43
|
|BUILDING_FACTORY
|-
|align="right"|44
|
|BUILDING_NUCLEAR_PLANT
|-
|align="right"|45
|
|BUILDING_SPACESHIP_FACTORY
|-
|align="right"|46
|
|BUILDING_MARKET
|-
|align="right"|47
|
|BUILDING_BANK
|-
|align="right"|48
|
|BUILDING_STOCK_EXCHANGE
|-
|align="right"|49
|
|BUILDING_LIBRARY
|-
|align="right"|50
|
|BUILDING_UNIVERSITY
|-
|align="right"|51
|
|BUILDING_PUBLIC_SCHOOL
|-
|align="right"|52
|
|BUILDING_LABORATORY
|-
|align="right"|53
|
|BUILDING_PALACE
|-
|align="right"|54
|
|BUILDING_HEROIC_EPIC
|-
|align="right"|55
|
|BUILDING_NATIONAL_COLLEGE
|-
|align="right"|56
|
|BUILDING_NATIONAL_EPIC
|-
|align="right"|57
|
|BUILDING_CIRCUS_MAXIMUS
|-
|align="right"|58
|
|BUILDING_NATIONAL_TREASURY
|-
|align="right"|59
|
|BUILDING_IRONWORKS
|-
|align="right"|60
|
|BUILDING_OXFORD_UNIVERSITY
|-
|align="right"|61
|
|BUILDING_HERMITAGE
|-
|align="right"|62
|
|BUILDING_GREAT_LIGHTHOUSE
|-
|align="right"|63
|
|BUILDING_STONEHENGE
|-
|align="right"|64
|
|BUILDING_GREAT_LIBRARY
|-
|align="right"|65
|
|BUILDING_PYRAMID
|-
|align="right"|66
|
|BUILDING_COLOSSUS
|-
|align="right"|67
|
|BUILDING_ORACLE
|-
|align="right"|68
|
|BUILDING_HANGING_GARDEN
|-
|align="right"|69
|
|BUILDING_GREAT_WALL
|-
|align="right"|70
|
|BUILDING_ANGKOR_WAT
|-
|align="right"|71
|
|BUILDING_HAGIA_SOPHIA
|-
|align="right"|72
|
|BUILDING_CHICHEN_ITZA
|-
|align="right"|73
|
|BUILDING_MACHU_PICHU
|-
|align="right"|74
|
|BUILDING_NOTRE_DAME
|-
|align="right"|75
|
|BUILDING_PORCELAIN_TOWER
|-
|align="right"|76
|
|BUILDING_HIMEJI_CASTLE
|-
|align="right"|77
|
|BUILDING_SISTINE_CHAPEL
|-
|align="right"|78
|
|BUILDING_KREMLIN
|-
|align="right"|79
|
|BUILDING_FORBIDDEN_PALACE
|-
|align="right"|80
|
|BUILDING_TAJ_MAHAL
|-
|align="right"|81
|
|BUILDING_BIG_BEN
|-
|align="right"|82
|
|BUILDING_LOUVRE
|-
|align="right"|83
|
|BUILDING_BRANDENBURG_GATE
|-
|align="right"|84
|
|BUILDING_STATUE_OF_LIBERTY
|-
|align="right"|85
|
|BUILDING_CRISTO_REDENTOR
|-
|align="right"|86
|
|BUILDING_EIFFEL_TOWER
|-
|align="right"|87
|
|BUILDING_PENTAGON
|-
|align="right"|88
|
|BUILDING_UNITED_NATIONS
|-
|align="right"|89
|
|BUILDING_SYDNEY_OPERA_HOUSE
|-
|align="right"|90
|
|BUILDING_AQUEDUCT
|-
|align="right"|91
|
|BUILDING_STONE_WORKS
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value -1. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Buildings.BUILDING_AMPHITHEATER.ID
local id = GameInfo["Buildings"].["BUILDING_AMPHITHEATER"].ID
local id = GameInfo.Buildings{Type="BUILDING_AMPHITHEATER"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_BUILDING_AMPHITHEATER.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Buildings[-1].Description
local description = GameInfo["Buildings"][-1]["Description"]
local description = GameInfo.Buildings{ID=-1}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETHELPTEXTFORBUILDING
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetHelpTextForBuilding}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' excludeName, '''bool''' excludeHeader, '''bool''' noMaintenance<b>)</b></code>
<!-- 
CANCONSTRUCT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanConstruct}}<b>(</b>{{Type5|BuildingType}} building, '''int''' continue, '''int''' testVisible, '''bool''' ignoreCost<b>)</b></code>
<!-- 
CHANGEBUILDINGPRODUCTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChangeBuildingProduction}}<b>(</b>{{Type5|BuildingType}} index, '''int''' change<b>)</b></code>
<!-- 
CHANGEBUILDINGPRODUCTIONTIME
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChangeBuildingProductionTime}}<b>(</b>{{Type5|BuildingType}} index, '''int''' change<b>)</b></code>
<!-- 
CHOOSEPRODUCTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChooseProduction}}<b>(</b>{{Type5|UnitType}} trainUnit, {{Type5|BuildingType}} constructBuilding, {{Type5|ProjectType}} createProject, '''bool''' finish, '''bool''' front<b>)</b></code>
<!-- 
GETBUILDINGESPIONAGEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingEspionageModifier}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETBUILDINGFAITHPURCHASECOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingFaithPurchaseCost}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' arg1 = nil<b>)</b></code>
<!-- 
GETBUILDINGGLOBALESPIONAGEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingGlobalEspionageModifier}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETBUILDINGORIGINALOWNER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingOriginalOwner}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGORIGINALTIME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingOriginalTime}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingProduction}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingProductionModifier}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONTIME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingProductionTime}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETBUILDINGPRODUCTIONTURNSLEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingProductionTurnsLeft}}<b>(</b>{{Type5|BuildingType}} building, '''int''' num<b>)</b></code>
<!-- 
GETBUILDINGPURCHASECOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingPurchaseCost}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETFIRSTBUILDINGORDER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetFirstBuildingOrder}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETLOCALRESOURCEWONDERPRODUCTIONMOD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetLocalResourceWonderProductionMod}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETNUMACTIVEBUILDING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumActiveBuilding}}<b>(</b>{{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
GETNUMBUILDING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumBuilding}}<b>(</b>{{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
GETNUMFREEBUILDING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumFreeBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETNUMREALBUILDING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumRealBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETNUMSPECIALISTSALLOWEDBYBUILDING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumSpecialistsAllowedByBuilding}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETNUMSPECIALISTSINBUILDING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumSpecialistsInBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETPRODUCTIONBUILDING
-->
|-
|align="right" width="200" |<code>{{Type5|BuildingType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProductionBuilding}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSELLBUILDINGREFUND
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSellBuildingRefund}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
GETTOTALBASEBUILDINGMAINTENANCE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetTotalBaseBuildingMaintenance}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
ISBUILDINGLOCALRESOURCEVALID
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsBuildingLocalResourceValid}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' checkForImprovement<b>)</b></code>
<!-- 
ISBUILDINGSELLABLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsBuildingSellable}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
ISCANADDSPECIALISTTOBUILDING
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsCanAddSpecialistToBuilding}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
ISHASBUILDING
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsHasBuilding}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
SETBUILDINGPRODUCTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetBuildingProduction}}<b>(</b>{{Type5|BuildingType}} index, '''int''' newValue<b>)</b></code>
<!-- 
SETBUILDINGPRODUCTIONTIME
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetBuildingProductionTime}}<b>(</b>{{Type5|BuildingType}} index, '''int''' newValue<b>)</b></code>
<!-- 
SETNUMREALBUILDING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetNumRealBuilding}}<b>(</b>{{Type5|BuildingType}} index, '''int''' newValue<b>)</b></code>
<!-- 
GETBUILDINGYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBuildingYieldChange}}<b>(</b>{{Type5|BuildingType}} building, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETBUILDINGYIELDMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBuildingYieldModifier}}<b>(</b>{{Type5|BuildingType}} building, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
ISBUILDINGEVERACTIVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsBuildingEverActive}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
SELECTEDCITIESGAMENETMESSAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SelectedCitiesGameNetMessage}}<b>(</b>{{Type5|GameMessageType}} message, {{Type5|TaskType}} data2, '''int''' data3, {{Type5|BuildingType}} data4, '''bool''' option, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
CITYBUILDINGSISBUILDINGSELLABLE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityBuildingsIsBuildingSellable}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|BuildingType}} building<b>)</b></code>
<!-- 
CITYCANCONSTRUCT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityCanConstruct}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
SENDSELLBUILDING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendSellBuilding}}<b>(</b>{{Type5|CityID}} arg0, {{Type5|BuildingType}} buildingToSell<b>)</b></code>
<!-- 
CANCONSTRUCT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanConstruct}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' continue, '''bool''' testVisible, '''bool''' ignoreCost<b>)</b></code>
<!-- 
COUNTNUMBUILDINGS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CountNumBuildings}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
GETADVANCEDSTARTBUILDINGCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartBuildingCost}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' add, {{Type5|City}} city<b>)</b></code>
<!-- 
GETBUILDINGCLASSPREREQBUILDING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetBuildingClassPrereqBuilding}}<b>(</b>{{Type5|BuildingType}} building, '''unknown''' ePrereqBuildingClass, '''int''' extra<b>)</b></code>
<!-- 
ISBUILDINGFREE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsBuildingFree}}<b>(</b>{{Type5|BuildingType}} building<b>)</b></code>
<!-- 
ISCANPURCHASEANYCITY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsCanPurchaseAnyCity}}<b>(</b>'''bool''' arg0, '''bool''' arg1, {{Type5|UnitType}} arg2, {{Type5|BuildingType}} arg3, {{Type5|YieldType}} arg4<b>)</b></code>
<!-- 
GETOBSOLETEBUILDINGCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetObsoleteBuildingCount}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
ISOBSOLETEBUILDING
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsObsoleteBuilding}}<b>(</b>{{Type5|BuildingType}} index<b>)</b></code>
<!-- 
CANCONSTRUCT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanConstruct}}<b>(</b>{{Type5|Plot}} plot, {{Type5|BuildingType}} building<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|BuildingType]]
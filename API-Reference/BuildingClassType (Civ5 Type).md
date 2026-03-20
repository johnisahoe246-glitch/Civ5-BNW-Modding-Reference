{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>BuildingClassType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>BuildingClassType</code> corresponds to the ''ID'' column of the {{Table5|BuildingClasses|CIV5BuildingClasses}} XML table.
}}


= XML: the BuildingClasses table =
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
|BUILDINGCLASS_COURTHOUSE
|-
|align="right"|0
|
|BUILDINGCLASS_CATHEDRAL
|-
|align="right"|1
|
|BUILDINGCLASS_SEAPORT
|-
|align="right"|1
|
|BUILDINGCLASS_MOSQUE
|-
|align="right"|2
|
|BUILDINGCLASS_STABLE
|-
|align="right"|2
|
|BUILDINGCLASS_PAGODA
|-
|align="right"|3
|
|BUILDINGCLASS_WATERMILL
|-
|align="right"|3
|
|BUILDINGCLASS_RECYCLING_CENTER
|-
|align="right"|4
|
|BUILDINGCLASS_CIRCUS
|-
|align="right"|4
|
|BUILDINGCLASS_BOMB_SHELTER
|-
|align="right"|5
|
|BUILDINGCLASS_FORGE
|-
|align="right"|5
|
|BUILDINGCLASS_CONSTABLE
|-
|align="right"|6
|
|BUILDINGCLASS_WINDMILL
|-
|align="right"|6
|
|BUILDINGCLASS_POLICE_STATION
|-
|align="right"|7
|
|BUILDINGCLASS_HYDRO_PLANT
|-
|align="right"|7
|
|BUILDINGCLASS_INTELLIGENCE_AGENCY
|-
|align="right"|8
|
|BUILDINGCLASS_SOLAR_PLANT
|-
|align="right"|8
|
|BUILDINGCLASS_ALHAMBRA
|-
|align="right"|9
|
|BUILDINGCLASS_MINT
|-
|align="right"|9
|
|BUILDINGCLASS_CN_TOWER
|-
|align="right"|10
|
|BUILDINGCLASS_OBSERVATORY
|-
|align="right"|10
|
|BUILDINGCLASS_HUBBLE
|-
|align="right"|11
|
|BUILDINGCLASS_MONASTERY
|-
|align="right"|11
|
|BUILDINGCLASS_LEANING_TOWER
|-
|align="right"|12
|
|BUILDINGCLASS_GARDEN
|-
|align="right"|12
|
|BUILDINGCLASS_MOSQUE_OF_DJENNE
|-
|align="right"|13
|
|BUILDINGCLASS_LIGHTHOUSE
|-
|align="right"|13
|
|BUILDINGCLASS_NEUSCHWANSTEIN
|-
|align="right"|14
|
|BUILDINGCLASS_HARBOR
|-
|align="right"|14
|
|BUILDINGCLASS_PETRA
|-
|align="right"|15
|
|BUILDINGCLASS_COLOSSEUM
|-
|align="right"|15
|
|BUILDINGCLASS_TERRACOTTA_ARMY
|-
|align="right"|16
|
|BUILDINGCLASS_THEATRE
|-
|align="right"|16
|
|BUILDINGCLASS_GREAT_FIREWALL
|-
|align="right"|17
|
|BUILDINGCLASS_STADIUM
|-
|align="right"|18
|
|BUILDINGCLASS_MONUMENT
|-
|align="right"|19
|
|BUILDINGCLASS_TEMPLE
|-
|align="right"|19
|
|BUILDINGCLASS_AMPHITHEATER
|-
|align="right"|20
|
|BUILDINGCLASS_OPERA_HOUSE
|-
|align="right"|21
|
|BUILDINGCLASS_MUSEUM
|-
|align="right"|22
|
|BUILDINGCLASS_BROADCAST_TOWER
|-
|align="right"|23
|
|BUILDINGCLASS_BARRACKS
|-
|align="right"|23
|
|BUILDINGCLASS_SHRINE
|-
|align="right"|24
|
|BUILDINGCLASS_ARMORY
|-
|align="right"|25
|
|BUILDINGCLASS_MILITARY_ACADEMY
|-
|align="right"|26
|
|BUILDINGCLASS_ARSENAL
|-
|align="right"|27
|
|BUILDINGCLASS_WALLS
|-
|align="right"|28
|
|BUILDINGCLASS_CASTLE
|-
|align="right"|29
|
|BUILDINGCLASS_MILITARY_BASE
|-
|align="right"|30
|
|BUILDINGCLASS_GRANARY
|-
|align="right"|31
|
|BUILDINGCLASS_HOSPITAL
|-
|align="right"|32
|
|BUILDINGCLASS_MEDICAL_LAB
|-
|align="right"|33
|
|BUILDINGCLASS_WORKSHOP
|-
|align="right"|34
|
|BUILDINGCLASS_FACTORY
|-
|align="right"|35
|
|BUILDINGCLASS_NUCLEAR_PLANT
|-
|align="right"|36
|
|BUILDINGCLASS_SPACESHIP_FACTORY
|-
|align="right"|37
|
|BUILDINGCLASS_MARKET
|-
|align="right"|38
|
|BUILDINGCLASS_BANK
|-
|align="right"|39
|
|BUILDINGCLASS_STOCK_EXCHANGE
|-
|align="right"|40
|
|BUILDINGCLASS_LIBRARY
|-
|align="right"|41
|
|BUILDINGCLASS_UNIVERSITY
|-
|align="right"|42
|
|BUILDINGCLASS_PUBLIC_SCHOOL
|-
|align="right"|43
|
|BUILDINGCLASS_LABORATORY
|-
|align="right"|44
|
|BUILDINGCLASS_PALACE
|-
|align="right"|45
|
|BUILDINGCLASS_HEROIC_EPIC
|-
|align="right"|46
|
|BUILDINGCLASS_NATIONAL_EPIC
|-
|align="right"|47
|
|BUILDINGCLASS_CIRCUS_MAXIMUS
|-
|align="right"|48
|
|BUILDINGCLASS_NATIONAL_TREASURY
|-
|align="right"|49
|
|BUILDINGCLASS_NATIONAL_COLLEGE
|-
|align="right"|50
|
|BUILDINGCLASS_IRONWORKS
|-
|align="right"|51
|
|BUILDINGCLASS_OXFORD_UNIVERSITY
|-
|align="right"|52
|
|BUILDINGCLASS_HERMITAGE
|-
|align="right"|53
|
|BUILDINGCLASS_PYRAMID
|-
|align="right"|54
|
|BUILDINGCLASS_GREAT_LIBRARY
|-
|align="right"|55
|
|BUILDINGCLASS_STONEHENGE
|-
|align="right"|56
|
|BUILDINGCLASS_HANGING_GARDEN
|-
|align="right"|57
|
|BUILDINGCLASS_COLOSSUS
|-
|align="right"|58
|
|BUILDINGCLASS_GREAT_LIGHTHOUSE
|-
|align="right"|59
|
|BUILDINGCLASS_ORACLE
|-
|align="right"|60
|
|BUILDINGCLASS_GREAT_WALL
|-
|align="right"|61
|
|BUILDINGCLASS_HAGIA_SOPHIA
|-
|align="right"|62
|
|BUILDINGCLASS_ANGKOR_WAT
|-
|align="right"|63
|
|BUILDINGCLASS_NOTRE_DAME
|-
|align="right"|64
|
|BUILDINGCLASS_MACHU_PICHU
|-
|align="right"|65
|
|BUILDINGCLASS_CHICHEN_ITZA
|-
|align="right"|66
|
|BUILDINGCLASS_KREMLIN
|-
|align="right"|67
|
|BUILDINGCLASS_FORBIDDEN_PALACE
|-
|align="right"|68
|
|BUILDINGCLASS_SISTINE_CHAPEL
|-
|align="right"|69
|
|BUILDINGCLASS_HIMEJI_CASTLE
|-
|align="right"|70
|
|BUILDINGCLASS_PORCELAIN_TOWER
|-
|align="right"|71
|
|BUILDINGCLASS_TAJ_MAHAL
|-
|align="right"|72
|
|BUILDINGCLASS_BIG_BEN
|-
|align="right"|73
|
|BUILDINGCLASS_BRANDENBURG_GATE
|-
|align="right"|74
|
|BUILDINGCLASS_LOUVRE
|-
|align="right"|75
|
|BUILDINGCLASS_EIFFEL_TOWER
|-
|align="right"|76
|
|BUILDINGCLASS_STATUE_OF_LIBERTY
|-
|align="right"|77
|
|BUILDINGCLASS_CRISTO_REDENTOR
|-
|align="right"|78
|
|BUILDINGCLASS_PENTAGON
|-
|align="right"|79
|
|BUILDINGCLASS_UNITED_NATIONS
|-
|align="right"|80
|
|BUILDINGCLASS_SYDNEY_OPERA_HOUSE
|-
|align="right"|81
|
|BUILDINGCLASS_AQUEDUCT
|-
|align="right"|82
|
|BUILDINGCLASS_STONE_WORKS
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.BuildingClasses.BUILDINGCLASS_CATHEDRAL.ID
local id = GameInfo["BuildingClasses"].["BUILDINGCLASS_CATHEDRAL"].ID
local id = GameInfo.BuildingClasses{Type="BUILDINGCLASS_CATHEDRAL"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_BUILDING_CATHEDRAL.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.BuildingClasses[0].Description
local description = GameInfo["BuildingClasses"][0]["Description"]
local description = GameInfo.BuildingClasses{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETBUILDINGYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetBuildingYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
GETRELIGIONBUILDINGCLASSHAPPINESS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetReligionBuildingClassHappiness}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETRELIGIONBUILDINGCLASSYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetReligionBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
SETBUILDINGYIELDCHANGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetBuildingYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} yield, '''int''' change<b>)</b></code>
<!-- 
GETBUILDINGCLASSCREATEDCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBuildingClassCreatedCount}}<b>(</b>{{Type5|BuildingClassType}} index<b>)</b></code>
<!-- 
ISBUILDINGCLASSMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsBuildingClassMaxedOut}}<b>(</b>{{Type5|BuildingClassType}} index, '''int''' extra<b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetBuildingClassCount}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNTPLUSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetBuildingClassCountPlusMaking}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetBuildingClassMaking}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETPLAYERBUILDINGCLASSHAPPINESS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPlayerBuildingClassHappiness}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETPLAYERBUILDINGCLASSYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPlayerBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETPOLICYBUILDINGCLASSYIELDCHANGE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPolicyBuildingClassYieldChange}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
GETPOLICYBUILDINGCLASSYIELDMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPolicyBuildingClassYieldModifier}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>
<!-- 
ISBUILDINGCLASSMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsBuildingClassMaxedOut}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, '''int''' extra<b>)</b></code>
<!-- 
ISPRODUCTIONMAXEDBUILDINGCLASS
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsProductionMaxedBuildingClass}}<b>(</b>{{Type5|BuildingClassType}} buildingClass, '''bool''' acquireCity<b>)</b></code>
<!-- 
REMOVEBUILDINGCLASS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|RemoveBuildingClass}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetBuildingClassCount}}<b>(</b>{{Type5|BuildingClassType}} index<b>)</b></code>
<!-- 
GETBUILDINGCLASSCOUNTPLUSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetBuildingClassCountPlusMaking}}<b>(</b>{{Type5|BuildingClassType}} unitClass<b>)</b></code>
<!-- 
GETBUILDINGCLASSMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetBuildingClassMaking}}<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>
<!-- 
ISBUILDINGCLASSMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsBuildingClassMaxedOut}}<b>(</b>{{Type5|BuildingClassType}} index, '''int''' extra<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|BuildingClassType]]
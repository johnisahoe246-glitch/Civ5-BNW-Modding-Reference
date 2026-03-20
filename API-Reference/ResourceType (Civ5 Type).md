{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ResourceType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ResourceType</code> corresponds to the ''ID'' column of the {{Table5|Resources|CIV5Resources}} XML table.
}}


= XML: the Resources table =
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
|RESOURCE_IRON
|-
|align="right"|1
|
|RESOURCE_HORSE
|-
|align="right"|2
|
|RESOURCE_COAL
|-
|align="right"|3
|
|RESOURCE_OIL
|-
|align="right"|4
|
|RESOURCE_ALUMINUM
|-
|align="right"|5
|
|RESOURCE_URANIUM
|-
|align="right"|6
|
|RESOURCE_WHEAT
|-
|align="right"|7
|
|RESOURCE_COW
|-
|align="right"|8
|
|RESOURCE_SHEEP
|-
|align="right"|9
|
|RESOURCE_DEER
|-
|align="right"|10
|
|RESOURCE_BANANA
|-
|align="right"|11
|
|RESOURCE_FISH
|-
|align="right"|12
|
|RESOURCE_STONE
|-
|align="right"|13
|
|RESOURCE_WHALE
|-
|align="right"|14
|
|RESOURCE_PEARLS
|-
|align="right"|15
|
|RESOURCE_GOLD
|-
|align="right"|16
|
|RESOURCE_SILVER
|-
|align="right"|17
|
|RESOURCE_GEMS
|-
|align="right"|18
|
|RESOURCE_MARBLE
|-
|align="right"|19
|
|RESOURCE_IVORY
|-
|align="right"|20
|
|RESOURCE_FUR
|-
|align="right"|21
|
|RESOURCE_DYE
|-
|align="right"|22
|
|RESOURCE_SPICES
|-
|align="right"|23
|
|RESOURCE_SILK
|-
|align="right"|24
|
|RESOURCE_SUGAR
|-
|align="right"|25
|
|RESOURCE_COTTON
|-
|align="right"|26
|
|RESOURCE_WINE
|-
|align="right"|27
|
|RESOURCE_INCENSE
|-
|align="right"|28
|
|RESOURCE_JEWELRY
|-
|align="right"|29
|
|RESOURCE_PORCELAIN
|-
|align="right"|30
|
|RESOURCE_COPPER
|-
|align="right"|31
|
|RESOURCE_SALT
|-
|align="right"|32
|
|RESOURCE_CRAB
|-
|align="right"|33
|
|RESOURCE_TRUFFLES
|-
|align="right"|34
|
|RESOURCE_CITRUS
|}</code>

40 RESOURCE_BISON

41 RESOURCE_COCOA
= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GRIDTOWORLD
-->
|-
|align="right" width="200" |<code>'''int''', '''int''', '''int'''</code>
|style="padding-left:6px" |<code>{{Func5|GridToWorld}}<b>(</b>{{Type5|ResourceType}} gridX, '''int''' gridY<b>)</b></code>
<!-- 
TOGRIDFROMHEX
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}, {{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Func5|ToGridFromHex}}<b>(</b>'''float''' i, '''float''' j<b>)</b></code>
<!-- 
GETNUMRESOURCES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetNumResources}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
ASSIGNLUXURYTOREGION
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|AssignLuxuryToRegion}}<b>(</b>{{Type5|PlayerID}} region_number<b>)</b></code>
<!-- 
CUSTOMOVERRIDE
-->
|-
|align="right" width="200" |<code>'''unknown''', '''int''', '''int''', '''int'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|CustomOverride}}<b>(</b>{{Type5|ResourceType}} resource_<b>)</b></code>
<!-- 
GETINDICESFORLUXURYTYPE
-->
|-
|align="right" width="200" |<code>'''int''', '''int''', '''int''', '''int'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|GetIndicesForLuxuryType}}<b>(</b>{{Type5|ResourceType}} resource_<b>)</b></code>
<!-- 
GETMAJORSTRATEGICRESOURCEQUANTITYVALUES
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|GetMajorStrategicResourceQuantityValues}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSMALLSTRATEGICRESOURCEQUANTITYVALUES
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|GetSmallStrategicResourceQuantityValues}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PLACESPECIFICNUMBEROFRESOURCES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|PlaceSpecificNumberOfResources}}<b>(</b>{{Type5|ResourceType}} resource_, {{Type5|ResourceType}} quantity, '''int''' amount, '''float''' ratio, '''int''' impact_table_number, '''int''' min_radius, '''int''' max_radius, table('''int''' => {{Type5|PlayerID}}) plot_list<b>)</b></code>
<!-- 
PROCESSRESOURCELIST
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|ProcessResourceList}}<b>(</b>'''int''' frequency, '''int''' impact_table_number, table('''int''' => '''int''') plot_list, table('''int''' => table('''int''' => {{Type5|ResourceType}})) resources_to_place<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Button}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} lClick, ('''void''' func<b>(</b>{{Type5|HandicapType}} index, {{Type5|ResourceType}} y, {{Type5|Button}} button, '''int''' x, '''int''' y<b>)</b>) OnEndTurnTimerClicked<b>)</b></code>
<!-- 
GETRESOURCEDEMANDED
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetResourceDemanded}}<b>(</b>'''bool''' arg0 = nil<b>)</b></code>
<!-- 
GETRESOURCEYIELDRATEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetResourceYieldRateModifier}}<b>(</b>{{Type5|YieldType}} index, {{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETX
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETY
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetY}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHASRESOURCELOCAL
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsHasResourceLocal}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
SETRESOURCEDEMANDED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|SetResourceDemanded}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
ADDCITYTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddCityTrade}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|ResourceType}} city<b>)</b></code>
<!-- 
ADDDEFENSIVEPACT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddDefensivePact}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDGOLDPERTURNTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddGoldPerTurnTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' goldPerTurn, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDOPENBORDERS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddOpenBorders}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDRESEARCHAGREEMENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddResearchAgreement}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDRESOURCETRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddResourceTrade}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resource, '''int''' amount, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDTRADEAGREEMENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|AddTradeAgreement}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
CHANGEGOLDPERTURNTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|ChangeGoldPerTurnTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' goldPerTurn, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
CHANGERESOURCETRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|ChangeResourceTrade}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resource, '''int''' numResource, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
GETNEXTITEM
-->
|-
|align="right" width="200" |<code>{{Type5|TradeableItemType}}, '''unknown''', '''unknown''', {{Type5|ResourceType}}, '''int''', {{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetNextItem}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|GetNumResource}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resType<b>)</b></code>
<!-- 
ISPOSSIBLETOTRADEITEM
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|IsPossibleToTradeItem}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them, {{Type5|TradeableItemType}} tradeType, {{Type5|TeamID}} dealDuration, {{Type5|ResourceType}} dealDuration = nil<b>)</b></code>
<!-- 
REMOVERESOURCETRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|RemoveResourceTrade}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
SETVOID2
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|EditBox}}:{{Func5|UIElement|SetVoid2}}<b>(</b>{{Type5|ResourceType}} arg0<b>)</b></code>
<!-- 
REQUESTYIELDDISPLAY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|RequestYieldDisplay}}<b>(</b>{{Type5|YieldDisplayType}} type, {{Type5|ResourceType}} arg1 = nil, {{Type5|ResourceType}} gridX = nil, '''int''' gridY = nil<b>)</b></code>
<!-- 
SERIALEVENTRAWRESOURCEICONCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventRawResourceIconCreated}}<b>(</b>'''float''' hexPosX, '''int''' hexPosY, '''unknown''' ImprovementType, {{Type5|ResourceType}} ResourceType<b>)</b></code>
<!-- 
SPAWNARROWEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SpawnArrowEvent}}<b>(</b>{{Type5|ResourceType}} arg0, {{Type5|ResourceType}} arg1, '''int''' hexX, '''int''' hexY<b>)</b></code>
<!-- 
GETDEALDURATION
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetDealDuration}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCEREQUIREDFORUNIT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetNumResourceRequiredForUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRESOURCEUSAGETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceUsageType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetResourceUsageType}}<b>(</b>{{Type5|ResourceType}} resourceLoop<b>)</b></code>
<!-- 
CITYCAPTURECOMPLETE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityCaptureComplete}}<b>(</b>{{Type5|PlayerID}} player, '''int''' capital, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|PlayerID}} newPlayer, '''int''' conquest, '''int''' conquest<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Grid}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} thisEvent, ('''void''' func<b>(</b>{{Type5|PlayerID}} void1, {{Type5|ResourceType}} void2, {{Type5|Button}} button<b>)</b>) OnContinueButtonClicked<b>)</b></code>
<!-- 
SETVOID2
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Grid}}:{{Func5|UIElement|SetVoid2}}<b>(</b>{{Type5|ResourceType}} numFreeTechs<b>)</b></code>
<!-- 
SETVOIDS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Grid}}:{{Func5|UIElement|SetVoids}}<b>(</b>{{Type5|TechType}} void1, {{Type5|ResourceType}} void2<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GridButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|PolicyType}} Id, {{Type5|ResourceType}} none, {{Type5|Button}} control<b>)</b>) OnEndTurnClicked<b>)</b></code>
<!-- 
SETVOIDS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GridButton}}:{{Func5|UIElement|SetVoids}}<b>(</b>{{Type5|ResourceType}} building, {{Type5|ResourceType}} addToList<b>)</b></code>
<!-- 
GETNUMRESOURCES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetNumResources}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETNUMRESOURCESONLAND
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetNumResourcesOnLand}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRANDOMRESOURCEQUANTITY
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetRandomResourceQuantity}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
SENDRESEARCH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendResearch}}<b>(</b>{{Type5|PlayerID}} tech, {{Type5|ResourceType}} discover, '''int''' value, '''bool''' arg3 = nil<b>)</b></code>
<!-- 
CHANGENUMRESOURCETOTAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|ChangeNumResourceTotal}}<b>(</b>{{Type5|ResourceType}} resource, '''int''' change<b>)</b></code>
<!-- 
GETHAPPINESSFROMLUXURY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetHappinessFromLuxury}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETNUMFREETECHS
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumFreeTechs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCEAVAILABLE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumResourceAvailable}}<b>(</b>{{Type5|ResourceType}} resource, '''bool''' includeImport<b>)</b></code>
<!-- 
GETNUMRESOURCETOTAL
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumResourceTotal}}<b>(</b>{{Type5|ResourceType}} resource, '''bool''' includeImport<b>)</b></code>
<!-- 
GETNUMRESOURCEUSED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetNumResourceUsed}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRESOURCEEXPORT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetResourceExport}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRESOURCEFROMMINORS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetResourceFromMinors}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETRESOURCEIMPORT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetResourceImport}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
INITUNIT
-->
|-
|align="right" width="200" |<code>{{Type5|Unit}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|InitUnit}}<b>(</b>{{Type5|UnitType}} unit, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|UnitAIType}} unitAI = NO_UNITAI, {{Type5|DirectionType}} facingDirection = NO_DIRECTION<b>)</b></code>
<!-- 
CANHAVERESOURCE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanHaveResource}}<b>(</b>{{Type5|ResourceType}} resource, '''bool''' ignoreLatitude<b>)</b></code>
<!-- 
GETNONOBSOLETERESOURCETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNonObsoleteResourceType}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
GETRESOURCETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetResourceType}}<b>(</b>{{Type5|TeamID}} team<b>)</b></code>
<!-- 
SETRESOURCETYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|SetResourceType}}<b>(</b>'''int''' newValue, {{Type5|ResourceType}} numResource<b>)</b></code>
<!-- 
GETVOID2
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Slider}}:{{Func5|UIElement|GetVoid2}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCENEEDEDTOUPGRADE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetNumResourceNeededToUpgrade}}<b>(</b>{{Type5|ResourceType}} resourceLoop<b>)</b></code>
<!-- 
GETX
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETY
-->
|-
|align="right" width="200" |<code>{{Type5|ResourceType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetY}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ResourceType]]
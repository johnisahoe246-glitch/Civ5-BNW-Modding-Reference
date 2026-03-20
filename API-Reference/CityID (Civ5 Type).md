{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CityID</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!}}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETID
-->
|-
|align="right" width="200" |<code>{{Type5|CityID}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
INITCITYRANGESTRIKE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|InitCityRangeStrike}}<b>(</b>{{Type5|PlayerID}} Player, {{Type5|CityID}} CityID<b>)</b></code>
<!-- 
SERIALEVENTCITYCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityCreated}}<b>(</b>{{Type5|Vector2}} vHexPos, {{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|ArtStyleType}} artStyleType, {{Type5|EraType}} eraType, '''int''' continent, '''int''' populationSize, '''int''' size, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTCITYSETDAMAGE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCitySetDamage}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, '''int''' damage, '''int''' previousDamage<b>)</b></code>
<!-- 
SPECIFICCITYINFODIRTY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SpecificCityInfoDirty}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|CityUpdateType}} updateType<b>)</b></code>
<!-- 
CITYCANCONSTRUCT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityCanConstruct}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|BuildingType}} buildingType<b>)</b></code>
<!-- 
SENDCITYBUYPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendCityBuyPlot}}<b>(</b>{{Type5|CityID}} arg0, '''int''' plotX, '''int''' plotY<b>)</b></code>
<!-- 
SENDDOTASK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendDoTask}}<b>(</b>{{Type5|CityID}} cityID, {{Type5|TaskType}} task, '''int''' plotIndex, '''int''' arg3, '''bool''' arg4, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>
<!-- 
SENDRENAMECITY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendRenameCity}}<b>(</b>{{Type5|CityID}} arg0, '''string''' arg1<b>)</b></code>
<!-- 
SENDSELLBUILDING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendSellBuilding}}<b>(</b>{{Type5|CityID}} arg0, {{Type5|BuildingType}} buildingToSell<b>)</b></code>
<!-- 
SENDSETCITYAIFOCUS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendSetCityAIFocus}}<b>(</b>{{Type5|CityID}} arg0, {{Type5|TaskType}} focus<b>)</b></code>
<!-- 
SENDSETCITYAVOIDGROWTH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendSetCityAvoidGrowth}}<b>(</b>{{Type5|CityID}} arg0, '''bool''' arg1<b>)</b></code>
<!-- 
SENDUPDATECITYCITIZENS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendUpdateCityCitizens}}<b>(</b>{{Type5|CityID}} arg0<b>)</b></code>
<!-- 
GETCITYBYID
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCityByID}}<b>(</b>{{Type5|CityID}} city<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CityID]]
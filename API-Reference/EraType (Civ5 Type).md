{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>EraType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>EraType</code> corresponds to the ''ID'' column of the {{Table5|Eras|CIV5Eras}} XML table.
}}


= XML: the Eras table =
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
|ERA_ANCIENT
|-
|align="right"|1
|
|ERA_CLASSICAL
|-
|align="right"|2
|
|ERA_MEDIEVAL
|-
|align="right"|3
|
|ERA_RENAISSANCE
|-
|align="right"|4
|
|ERA_INDUSTRIAL
|-
|align="right"|5
|
|ERA_MODERN
|-
|align="right"|6
|
|ERA_FUTURE
|-
|align="right"|6
|
|ERA_POSTMODERN
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SERIALEVENTCITYCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityCreated}}<b>(</b>{{Type5|Vector2}} vHexPos, {{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|ArtStyleType}} artStyleType, {{Type5|EraType}} eraType, '''int''' continent, '''int''' populationSize, '''int''' size, '''int''' fogState<b>)</b></code>
<!-- 
GETCURRENTERA
-->
|-
|align="right" width="200" |<code>{{Type5|EraType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetCurrentEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTARTERA
-->
|-
|align="right" width="200" |<code>{{Type5|EraType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetStartEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSUPPORTEDLANGUAGES
-->
|-
|align="right" width="200" |<code>table({{Type5|EraType}} => {{Type5|ModInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Locale}}.{{Func5|Locale|GetSupportedLanguages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSUPPORTEDSPOKENLANGUAGES
-->
|-
|align="right" width="200" |<code>table({{Type5|EraType}} => {{Type5|ModInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Locale}}.{{Func5|Locale|GetSupportedSpokenLanguages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRESOLUTION_CACHED
-->
|-
|align="right" width="200" |<code>{{Type5|EraType}}</code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|GetResolution_Cached}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETBINDMOUSEMODE_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetBindMouseMode_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETFOWLEVEL_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetFOWLevel_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETLEADERQUALITY_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetLeaderQuality_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETOVERLAYLEVEL_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetOverlayLevel_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETRESOLUTION_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetResolution_Cached}}<b>(</b>{{Type5|EraType}} fullscreenRes<b>)</b></code>
<!-- 
SETSHADOWLEVEL_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetShadowLevel_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETTERRAINDETAILLEVEL_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetTerrainDetailLevel_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETTERRAINSHADOWQUALITY_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetTerrainShadowQuality_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETTERRAINTESSLEVEL_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetTerrainTessLevel_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETTEXTUREQUALITY_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetTextureQuality_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
SETWATERQUALITY_CACHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|OptionsManager}}.{{Func5|OptionsManager|SetWaterQuality_Cached}}<b>(</b>{{Type5|EraType}} level<b>)</b></code>
<!-- 
GETCURRENTERA
-->
|-
|align="right" width="200" |<code>{{Type5|EraType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCurrentEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETERA
-->
|-
|align="right" width="200" |<code>{{Type5|EraType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETERA
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetEra}}<b>(</b>{{Type5|EraType}} id<b>)</b></code>
<!-- 
GETRESINFO
-->
|-
|align="right" width="200" |<code>'''int''', '''int''', '''unknown''', '''unknown''', '''unknown''', '''int'''</code>
|style="padding-left:6px" |<code>{{Type5|UIManager}}.{{Func5|UIManager|GetResInfo}}<b>(</b>{{Type5|EraType}} i<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|EraType]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ArtStyleType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ArtStyleType</code> corresponds to the ''ID'' column of the {{Table5|ArtStyleTypes|CIV5ArtStyleTypes}} XML table.
}}


= XML: the ArtStyleTypes table =
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
|ARTSTYLE_SOUTH_AMERICA
|-
|align="right"|1
|
|ARTSTYLE_ASIAN
|-
|align="right"|2
|
|ARTSTYLE_MIDDLE_EAST
|-
|align="right"|3
|
|ARTSTYLE_EUROPEAN
|-
|align="right"|4
|
|ARTSTYLE_GRECO_ROMAN
|-
|align="right"|5
|
|ARTSTYLE_POLYNESIAN
|-
|align="right"|6
|
|ARTSTYLE_BARBARIAN
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.ArtStyleTypes.ARTSTYLE_SOUTH_AMERICA.ID
local id = GameInfo["ArtStyleTypes"].["ARTSTYLE_SOUTH_AMERICA"].ID
local id = GameInfo.ArtStyleTypes{Type="ARTSTYLE_SOUTH_AMERICA"}().ID
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETARTSTYLETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ArtStyleType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetArtStyleType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTCITYCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityCreated}}<b>(</b>{{Type5|Vector2}} vHexPos, {{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|ArtStyleType}} artStyleType, {{Type5|EraType}} eraType, '''int''' continent, '''int''' populationSize, '''int''' size, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTIMPROVEMENTCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventImprovementCreated}}<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent1, {{Type5|ArtStyleType}} continent2, {{Type5|PlayerID}} player, '''int''' createImprovementType, {{Type5|ImprovementType}} createImprovementRRType, '''int''' createImprovementEra, '''int''' createImprovementState, '''unknown''' ImprovementEra = nil<b>)</b></code>
<!-- 
SERIALEVENTRAWRESOURCECREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventRawResourceCreated}}<b>(</b>'''float''' hexX, '''int''' hexY, {{Type5|ArtStyleType}} continent, {{Type5|ArtStyleType}} continent, {{Type5|PlayerID}} player, '''int''' arg5, '''int''' createResourceType, '''int''' arg7, '''int''' arg8<b>)</b></code>
<!-- 
GETARTSTYLETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ArtStyleType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetArtStyleType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCONTINENTARTTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|ArtStyleType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetContinentArtType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETCONTINENTARTTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|SetContinentArtType}}<b>(</b>{{Type5|ArtStyleType}} style<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ArtStyleType]]
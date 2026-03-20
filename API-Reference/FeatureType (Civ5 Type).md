{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>FeatureType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>FeatureType</code> corresponds to the ''ID'' column of the {{Table5|Features|CIV5Features}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''FeatureTypes''' Lua enumeration.
}}


= Lua: the FeatureTypes enumeration =
Firaxis provides a Lua enumeration named <code>FeatureTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Features|CIV5Features}} data table.<br/>
* They are stored as key/value pairs: the keys are the strings from the ''Type'' column and the values are the integers from the ''ID'' column.<br/>
{{Warning}} Be careful: this enumeration do '''not''' reflect the changes, additions and deletions made by mods. As a result it is advised to rely on {{Type5|GameInfo}} instead.<br/>

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_FEATURE"
|
|align="right" |-1
|-
|align="left" |"FEATURE_ICE"
|
|align="right" |0
|-
|align="left" |"FEATURE_JUNGLE"
|
|align="right" |1
|-
|align="left" |"FEATURE_MARSH"
|
|align="right" |2
|-
|align="left" |"FEATURE_OASIS"
|
|align="right" |3
|-
|align="left" |"FEATURE_FLOOD_PLAINS"
|
|align="right" |4
|-
|align="left" |"FEATURE_FOREST"
|
|align="right" |5
|-
|align="left" |"FEATURE_FALLOUT"
|
|align="right" |6
|-
|align="left" |"NUM_FEATURE_TYPES"
|
|align="right" |8
|}</code>


= XML: the Features table =
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
|FEATURE_ICE
|-
|align="right"|1
|
|FEATURE_JUNGLE
|-
|align="right"|2
|
|FEATURE_MARSH
|-
|align="right"|3
|
|FEATURE_OASIS
|-
|align="right"|4
|
|FEATURE_FLOOD_PLAINS
|-
|align="right"|5
|
|FEATURE_FOREST
|-
|align="right"|6
|
|FEATURE_FALLOUT
|-
|align="right"|7
|
|FEATURE_CRATER
|-
|align="right"|8
|
|FEATURE_FUJI
|-
|align="right"|9
|
|FEATURE_MESA
|-
|align="right"|10
|
|FEATURE_REEF
|-
|align="right"|11
|
|FEATURE_VOLCANO
|-
|align="right"|12
|
|FEATURE_GIBRALTAR
|-
|align="right"|13
|
|FEATURE_GEYSER
|-
|align="right"|14
|
|FEATURE_FOUNTAIN_YOUTH
|-
|align="right"|15
|
|FEATURE_POTOSI
|-
|align="right"|16
|
|FEATURE_EL_DORADO
|-
|align="right"|17
|
|FEATURE_ATOLL
|-
|align="right"|18
|
|FEATURE_SRI_PADA
|-
|align="right"|19
|
|FEATURE_MT_SINAI
|-
|align="right"|20
|
|FEATURE_MT_KAILASH
|-
|align="right"|21
|
|FEATURE_ULURU
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = FeatureTypes.FEATURE_ICE
local id = FeatureTypes["FEATURE_ICE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ISFEATURESPECIAL
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Func5|IsFeatureSpecial}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
GENERICWORLDANCHOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|GenericWorldAnchor}}<b>(</b>{{Type5|GenericWorldAnchorType}} type, '''bool''' show, '''int''' plotX, '''int''' plotY, {{Type5|FeatureType}} data1 = nil<b>)</b></code>
<!-- 
COUNTCITYFEATURES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CountCityFeatures}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
ISBUILDBLOCKEDBYFEATURE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsBuildBlockedByFeature}}<b>(</b>{{Type5|BuildActionType}} build, {{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
CANHAVEFEATURE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|CanHaveFeature}}<b>(</b>{{Type5|FeatureType}} featureForest<b>)</b></code>
<!-- 
GETFEATURETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|FeatureType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetFeatureType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
FEATUREATTACKMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|FeatureAttackModifier}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
FEATUREDEFENSEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|FeatureDefenseModifier}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
<!-- 
GETEXTRAFEATUREATTACKPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetExtraFeatureAttackPercent}}<b>(</b>{{Type5|FeatureType}} index<b>)</b></code>
<!-- 
GETEXTRAFEATUREDEFENSEPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetExtraFeatureDefensePercent}}<b>(</b>{{Type5|FeatureType}} index<b>)</b></code>
<!-- 
ISFEATUREDOUBLEMOVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsFeatureDoubleMove}}<b>(</b>{{Type5|FeatureType}} index<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|FeatureType]]
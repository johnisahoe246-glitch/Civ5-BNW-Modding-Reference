{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>TerrainType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>TerrainType</code> corresponds to the ''ID'' column of the {{Table5|Terrains|CIV5Terrains}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''TerrainTypes''' Lua enumeration.
}}


= Lua: the TerrainTypes enumeration =
Firaxis provides a Lua enumeration named <code>TerrainTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Terrains|CIV5Terrains}} data table.<br/>
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
|align="left" |"NO_TERRAIN"
|
|align="right" |-1
|-
|align="left" |"TERRAIN_GRASS"
|
|align="right" |0
|-
|align="left" |"TERRAIN_PLAINS"
|
|align="right" |1
|-
|align="left" |"TERRAIN_DESERT"
|
|align="right" |2
|-
|align="left" |"TERRAIN_TUNDRA"
|
|align="right" |3
|-
|align="left" |"TERRAIN_SNOW"
|
|align="right" |4
|-
|align="left" |"TERRAIN_COAST"
|
|align="right" |5
|-
|align="left" |"TERRAIN_OCEAN"
|
|align="right" |6
|-
|align="left" |"TERRAIN_MOUNTAIN"
|
|align="right" |7
|-
|align="left" |"TERRAIN_HILL"
|
|align="right" |8
|-
|align="left" |"NUM_TERRAIN_TYPES"
|
|align="right" |9
|}</code>


= XML: the Terrains table =
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
|TERRAIN_GRASS
|-
|align="right"|1
|
|TERRAIN_PLAINS
|-
|align="right"|2
|
|TERRAIN_DESERT
|-
|align="right"|3
|
|TERRAIN_TUNDRA
|-
|align="right"|4
|
|TERRAIN_SNOW
|-
|align="right"|5
|
|TERRAIN_COAST
|-
|align="right"|6
|
|TERRAIN_OCEAN
|-
|align="right"|7
|
|TERRAIN_MOUNTAIN
|-
|align="right"|8
|
|TERRAIN_HILL
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = TerrainTypes.TERRAIN_GRASS
local id = TerrainTypes["TERRAIN_GRASS"]
</syntaxhighlight>
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Terrains.TERRAIN_GRASS.ID
local id = GameInfo["Terrains"].["TERRAIN_GRASS"].ID
local id = GameInfo.Terrains{Type="TERRAIN_GRASS"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_TERRAIN_GRASS.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Terrains[0].Description
local description = GameInfo["Terrains"][0]["Description"]
local description = GameInfo.Terrains{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SETTERRAINTYPES
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Func5|SetTerrainTypes}}<b>(</b>table('''int''' => {{Type5|TerrainType}}) terrainTypes<b>)</b></code>
<!-- 
GETTERRAINTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|TerrainType}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetTerrainType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETTERRAINTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|SetTerrainType}}<b>(</b>{{Type5|TerrainType}} terrain, '''bool''' recalculateAreas, '''bool''' rebuildGraphics)<b>)</b></code>
<!-- 
SETPLOT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|ReplayMap}}:{{Func5|UIElement|SetPlot}}<b>(</b>'''int''' x, '''int''' y, {{Type5|TerrainType}} terrain, '''int''' r, '''int''' g, '''int''' b, '''int''' a<b>)</b></code>
<!-- 
GENERATETERRAIN
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|TerrainType}})</code>
|style="padding-left:6px" |<code>{{Type5|TerrainGenerator}}:{{Func5|TerrainGenerator|GenerateTerrain}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRATERRAINATTACKPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetExtraTerrainAttackPercent}}<b>(</b>{{Type5|TerrainType}} index<b>)</b></code>
<!-- 
GETEXTRATERRAINDEFENSEPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetExtraTerrainDefensePercent}}<b>(</b>{{Type5|TerrainType}} index<b>)</b></code>
<!-- 
ISTERRAINDOUBLEMOVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsTerrainDoubleMove}}<b>(</b>{{Type5|TerrainType}} index<b>)</b></code>
<!-- 
TERRAINATTACKMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|TerrainAttackModifier}}<b>(</b>{{Type5|TerrainType}} terrain<b>)</b></code>
<!-- 
TERRAINDEFENSEMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|TerrainDefenseModifier}}<b>(</b>{{Type5|TerrainType}} terrain<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|TerrainType]]
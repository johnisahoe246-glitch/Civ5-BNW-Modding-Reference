{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>HurryType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>HurryType</code> corresponds to the ''ID'' column of the {{Table5|HurryInfos|CIV5HurryInfos}} XML table.
}}


= XML: the HurryInfos table =
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
|HURRY_POPULATION
|-
|align="right"|1
|
|HURRY_GOLD
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.HurryInfos.HURRY_POPULATION.ID
local id = GameInfo["HurryInfos"].["HURRY_POPULATION"].ID
local id = GameInfo.HurryInfos{Type="HURRY_POPULATION"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_HURRY_POPULATION.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.HurryInfos[0].Description
local description = GameInfo["HurryInfos"][0]["Description"]
local description = GameInfo.HurryInfos{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANHURRY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanHurry}}<b>(</b>{{Type5|HurryType}} hurry, '''bool''' testVisible<b>)</b></code>
<!-- 
HURRY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|Hurry}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
HURRYCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|HurryCost}}<b>(</b>{{Type5|HurryType}} hurry, '''bool''' extra<b>)</b></code>
<!-- 
HURRYGOLD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|HurryGold}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
HURRYPOPULATION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|HurryPopulation}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
HURRYPRODUCTION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|HurryProduction}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETPRODUCTIONPERPOPULATION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetProductionPerPopulation}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETHURRYCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetHurryCount}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETHURRYGOLDCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetHurryGoldCost}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
GETHURRYMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetHurryModifier}}<b>(</b>{{Type5|HurryType}} hurry<b>)</b></code>
<!-- 
ISCANHURRY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsCanHurry}}<b>(</b>{{Type5|HurryType}} index<b>)</b></code>
<!-- 
ISHASACCESSTOHURRY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsHasAccessToHurry}}<b>(</b>{{Type5|HurryType}} index<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|HurryType]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ClimateType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ClimateType</code> corresponds to the ''ID'' column of the {{Table5|Climates|CIV5Climates}} XML table.
}}


= XML: the Climates table =
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
|CLIMATE_TEMPERATE
|-
|align="right"|1
|
|CLIMATE_TROPICAL
|-
|align="right"|2
|
|CLIMATE_ARID
|-
|align="right"|3
|
|CLIMATE_ROCKY
|-
|align="right"|4
|
|CLIMATE_COLD
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Climates.CLIMATE_TEMPERATE.ID
local id = GameInfo["Climates"].["CLIMATE_TEMPERATE"].ID
local id = GameInfo.Climates{Type="CLIMATE_TEMPERATE"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_CLIMATE_TEMPERATE.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Climates[0].Description
local description = GameInfo["Climates"][0]["Description"]
local description = GameInfo.Climates{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCLIMATE
-->
|-
|align="right" width="200" |<code>{{Type5|ClimateType}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetClimate}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ClimateType]]
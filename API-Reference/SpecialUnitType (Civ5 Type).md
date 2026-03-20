{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>SpecialUnitType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>SpecialUnitType</code> corresponds to the ''ID'' column of the {{Table5|SpecialUnits|CIV5SpecialUnits}} XML table.
}}


= XML: the SpecialUnits table =
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
|SPECIALUNIT_FIGHTER
|-
|align="right"|1
|
|SPECIALUNIT_PEOPLE
|-
|align="right"|2
|
|SPECIALUNIT_MISSILE
|-
|align="right"|3
|
|SPECIALUNIT_STEALTH
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.SpecialUnits.SPECIALUNIT_FIGHTER.ID
local id = GameInfo["SpecialUnits"].["SPECIALUNIT_FIGHTER"].ID
local id = GameInfo.SpecialUnits{Type="SPECIALUNIT_FIGHTER"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_SPECIALUNIT_FIGHTER.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.SpecialUnits[0].Description
local description = GameInfo["SpecialUnits"][0]["Description"]
local description = GameInfo.SpecialUnits{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ISSPECIALUNITVALID
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsSpecialUnitValid}}<b>(</b>{{Type5|SpecialUnitType}} specialUnitType<b>)</b></code>
<!-- 
MAKESPECIALUNITVALID
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|MakeSpecialUnitValid}}<b>(</b>{{Type5|SpecialUnitType}} specialUnitType<b>)</b></code>
<!-- 
CARGOSPACEAVAILABLE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CargoSpaceAvailable}}<b>(</b>{{Type5|SpecialUnitType}} specialCargo, {{Type5|DomainType}} domainCargo<b>)</b></code>
<!-- 
GETSPECIALUNITTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|SpecialUnitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetSpecialUnitType}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|SpecialUnitType]]
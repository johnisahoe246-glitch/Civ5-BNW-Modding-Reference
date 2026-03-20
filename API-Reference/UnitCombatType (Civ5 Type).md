{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>UnitCombatType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>UnitCombatType</code> corresponds to the ''ID'' column of the {{Table5|UnitCombatInfos|CIV5UnitCombatInfos}} XML table.
}}


= XML: the UnitCombatInfos table =
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
|UNITCOMBAT_RECON
|-
|align="right"|1
|
|UNITCOMBAT_ARCHER
|-
|align="right"|2
|
|UNITCOMBAT_MOUNTED
|-
|align="right"|3
|
|UNITCOMBAT_MELEE
|-
|align="right"|4
|
|UNITCOMBAT_SIEGE
|-
|align="right"|5
|
|UNITCOMBAT_GUN
|-
|align="right"|6
|
|UNITCOMBAT_ARMOR
|-
|align="right"|7
|
|UNITCOMBAT_HELICOPTER
|-
|align="right"|8
|
|UNITCOMBAT_NAVAL
|-
|align="right"|8
|
|UNITCOMBAT_NAVALRANGED
|-
|align="right"|9
|
|UNITCOMBAT_FIGHTER
|-
|align="right"|10
|
|UNITCOMBAT_BOMBER
|-
|align="right"|11
|
|UNITCOMBAT_NAVALMELEE
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETUNITCOMBATFREEEXPERIENCE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetUnitCombatFreeExperience}}<b>(</b>{{Type5|UnitCombatType}} index<b>)</b></code>
<!-- 
GETEXTRAUNITCOMBATMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetExtraUnitCombatModifier}}<b>(</b>{{Type5|UnitCombatType}} index<b>)</b></code>
<!-- 
GETUNITCOMBATTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|UnitCombatType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetUnitCombatType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
UNITCOMBATMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|UnitCombatModifier}}<b>(</b>{{Type5|UnitCombatType}} unitCombat<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|UnitCombatType]]
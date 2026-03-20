{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GoodyType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>GoodyType</code> corresponds to the ''ID'' column of the {{Table5|GoodyHuts|CIV5GoodyHuts}} XML table.
}}


= XML: the GoodyHuts table =
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
|GOODY_WARRIOR
|-
|align="right"|1
|
|GOODY_POPULATION
|-
|align="right"|2
|
|GOODY_CULTURE
|-
|align="right"|3
|
|GOODY_REVEAL_NEARBY_BARBS
|-
|align="right"|3
|
|GOODY_PANTHEON_FAITH
|-
|align="right"|4
|
|GOODY_GOLD
|-
|align="right"|4
|
|GOODY_PROPHET_FAITH
|-
|align="right"|5
|
|GOODY_MAP
|-
|align="right"|6
|
|GOODY_TECH
|-
|align="right"|7
|
|GOODY_REVEAL_RESOURCE
|-
|align="right"|8
|
|GOODY_UPGRADE_UNIT
|-
|align="right"|9
|
|GOODY_BARBARIANS_WEAK
|-
|align="right"|10
|
|GOODY_BARBARIANS_STRONG
|-
|align="right"|11
|
|GOODY_LOW_GOLD
|-
|align="right"|12
|
|GOODY_HIGH_GOLD
|-
|align="right"|13
|
|GOODY_SETTLER
|-
|align="right"|14
|
|GOODY_SCOUT
|-
|align="right"|15
|
|GOODY_WORKER
|-
|align="right"|16
|
|GOODY_EXPERIENCE
|-
|align="right"|17
|
|GOODY_HEALING
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANRECEIVEGOODY
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
<!-- 
RECEIVEGOODY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|ReceiveGoody}}<b>(</b>{{Type5|Plot}} plot, {{Type5|GoodyType}} goody, {{Type5|Unit}} unit<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GoodyType]]
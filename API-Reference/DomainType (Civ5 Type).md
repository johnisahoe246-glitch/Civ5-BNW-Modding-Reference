{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>DomainType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>DomainType</code> corresponds to the ''ID'' column of the {{Table5|Domains|CIV5Domains}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''DomainTypes''' Lua enumeration.
}}


= Lua: the DomainTypes enumeration =
Firaxis provides a Lua enumeration named <code>DomainTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Domains|CIV5Domains}} data table.<br/>
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
|align="left" |"NO_DOMAIN"
|
|align="right" |-1
|-
|align="left" |"DOMAIN_SEA"
|
|align="right" |0
|-
|align="left" |"DOMAIN_AIR"
|
|align="right" |1
|-
|align="left" |"DOMAIN_LAND"
|
|align="right" |2
|-
|align="left" |"DOMAIN_IMMOBILE"
|
|align="right" |3
|-
|align="left" |"DOMAIN_HOVER"
|
|align="right" |4
|-
|align="left" |"NUM_DOMAIN_TYPES"
|
|align="right" |5
|}</code>


= XML: the Domains table =
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
|DOMAIN_SEA
|-
|align="right"|1
|
|DOMAIN_AIR
|-
|align="right"|2
|
|DOMAIN_LAND
|-
|align="right"|3
|
|DOMAIN_IMMOBILE
|-
|align="right"|4
|
|DOMAIN_HOVER
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = DomainTypes.DOMAIN_SEA
local id = DomainTypes["DOMAIN_SEA"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETDOMAINFREEEXPERIENCE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetDomainFreeExperience}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
<!-- 
GETDOMAINPRODUCTIONMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetDomainProductionModifier}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
<!-- 
CHANGEEXTRAMOVES
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|ChangeExtraMoves}}<b>(</b>{{Type5|DomainType}} index, '''int''' change<b>)</b></code>
<!-- 
GETEXTRAMOVES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetExtraMoves}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
<!-- 
CARGOSPACEAVAILABLE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CargoSpaceAvailable}}<b>(</b>{{Type5|SpecialUnitType}} specialCargo, {{Type5|DomainType}} domainCargo<b>)</b></code>
<!-- 
DOMAINCARGO
-->
|-
|align="right" width="200" |<code>{{Type5|DomainType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|DomainCargo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOMAINMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|DomainModifier}}<b>(</b>{{Type5|DomainType}} domain<b>)</b></code>
<!-- 
GETDOMAINTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|DomainType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetDomainType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTRADOMAINMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetExtraDomainModifier}}<b>(</b>{{Type5|DomainType}} index<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|DomainType]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MinorCivTraitType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>MinorCivTraitType</code> corresponds to the ''ID'' column of the {{Table5|MinorCivTraits|CIV5MinorCivTraits}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''MinorCivTraitTypes''' Lua enumeration.
}}


= Lua: the MinorCivTraitTypes enumeration =
Firaxis provides a Lua enumeration named <code>MinorCivTraitTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|MinorCivTraits|CIV5MinorCivTraits}} data table.<br/>
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
|align="left" |"NO_MINOR_CIV_TRAIT_TYPE"
|
|align="right" |-1
|-
|align="left" |"MINOR_CIV_TRAIT_CULTURED"
|
|align="right" |0
|-
|align="left" |"MINOR_CIV_TRAIT_MILITARISTIC"
|
|align="right" |1
|-
|align="left" |"MINOR_CIV_TRAIT_MARITIME"
|
|align="right" |2
|-
|align="left" |"MINOR_CIV_TRAIT_MERCANTILE"
|
|align="right" |3
|-
|align="left" |"MINOR_CIV_TRAIT_RELIGIOUS"
|
|align="right" |4
|-
|align="left" |"NUM_MINOR_CIV_TRAIT_TYPES"
|
|align="right" |5
|}</code>


= XML: the MinorCivTraits table =
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
|MINOR_TRAIT_CULTURED
|-
|align="right"|1
|
|MINOR_TRAIT_MILITARISTIC
|-
|align="right"|2
|
|MINOR_TRAIT_MARITIME
|-
|align="right"|3
|
|MINOR_TRAIT_MERCANTILE
|-
|align="right"|4
|
|MINOR_TRAIT_RELIGIOUS
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = MinorCivTraitTypes.MINOR_CIV_TRAIT_CULTURED
local id = MinorCivTraitTypes["MINOR_CIV_TRAIT_CULTURED"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETMINORCIVTRAIT
-->
|-
|align="right" width="200" |<code>{{Type5|MinorCivTraitType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetMinorCivTrait}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MinorCivTraitType]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>FaithPurchaseType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>FaithPurchaseType</code> corresponds to the constants defined in the '''FaithPurchaseTypes''' Lua enumeration.
}}


= Lua: the FaithPurchaseTypes enumeration =
Firaxis provides a Lua enumeration named <code>FaithPurchaseTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_AUTOMATIC_FAITH_PURCHASE"
|
|align="right" |0
|-
|align="left" |"FAITH_PURCHASE_SAVE_PROPHET"
|
|align="right" |1
|-
|align="left" |"FAITH_PURCHASE_BUILDING"
|
|align="right" |2
|-
|align="left" |"FAITH_PURCHASE_UNIT"
|
|align="right" |3
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = FaithPurchaseTypes.NO_AUTOMATIC_FAITH_PURCHASE
local id = FaithPurchaseTypes["NO_AUTOMATIC_FAITH_PURCHASE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
REGISTERSELECTIONCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>ControlBase:{{Func5|UIElement|RegisterSelectionCallback}}<b>(</b>('''void''' func<b>(</b>{{Type5|FaithPurchaseType}} v1, '''int''' v2<b>)</b>) OnChatTarget<b>)</b></code>
<!-- 
SENDFAITHPURCHASE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFaithPurchase}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|FaithPurchaseType}} v1, '''int''' v2<b>)</b></code>
<!-- 
GETFAITHPURCHASETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|FaithPurchaseType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetFaithPurchaseType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETFAITHPURCHASETYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetFaithPurchaseType}}<b>(</b>{{Type5|FaithPurchaseType}} v1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|FaithPurchaseType]]
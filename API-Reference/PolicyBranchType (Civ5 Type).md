{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>PolicyBranchType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>PolicyBranchType</code> corresponds to the ''ID'' column of the {{Table5|PolicyBranchTypes|CIV5PolicyBranchTypes}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''PolicyBranchTypes''' Lua enumeration.
}}


= Lua: the PolicyBranchTypes enumeration =
Firaxis provides a Lua enumeration named <code>PolicyBranchTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|PolicyBranchTypes|CIV5PolicyBranchTypes}} data table.<br/>
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
|align="left" |"NO_POLICY_BRANCH_TYPE"
|
|align="right" |-1
|}</code>


= XML: the PolicyBranchTypes table =
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
|POLICY_BRANCH_TRADITION
|-
|align="right"|1
|
|POLICY_BRANCH_LIBERTY
|-
|align="right"|2
|
|POLICY_BRANCH_HONOR
|-
|align="right"|3
|
|POLICY_BRANCH_PIETY
|-
|align="right"|4
|
|POLICY_BRANCH_PATRONAGE
|-
|align="right"|5
|
|POLICY_BRANCH_COMMERCE
|-
|align="right"|6
|
|POLICY_BRANCH_RATIONALISM
|-
|align="right"|7
|
|POLICY_BRANCH_FREEDOM
|-
|align="right"|8
|
|POLICY_BRANCH_ORDER
|-
|align="right"|9
|
|POLICY_BRANCH_AUTOCRACY
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value -1.
<syntaxhighlight lang="lua" class="civ5-example">
local id = PolicyBranchTypes.NO_POLICY_BRANCH_TYPE
local id = PolicyBranchTypes["NO_POLICY_BRANCH_TYPE"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETDOMINANTPOLICYBRANCHFORTITLE
-->
|-
|align="right" width="200" |<code>{{Type5|PolicyBranchType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetDominantPolicyBranchForTitle}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPOLICYBRANCHBLOCKED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPolicyBranchBlocked}}<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex<b>)</b></code>
<!-- 
ISPOLICYBRANCHFINISHED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPolicyBranchFinished}}<b>(</b>{{Type5|PolicyBranchType}} arg0<b>)</b></code>
<!-- 
ISPOLICYBRANCHUNLOCKED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPolicyBranchUnlocked}}<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex<b>)</b></code>
<!-- 
SETPOLICYBRANCHUNLOCKED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetPolicyBranchUnlocked}}<b>(</b>{{Type5|PolicyBranchType}} arg0, '''bool''' arg1<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TextButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} OnSearchTextEnter, ('''void''' func<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex, {{Type5|UnitType}} y, {{Type5|Button}} button<b>)</b>) OnClose = nil<b>)</b></code>
<!-- 
SETUICURSOR
-->
|-
|align="right" width="200" |<code>{{Type5|PolicyBranchType}}</code>
|style="padding-left:6px" |<code>{{Type5|UIManager}}.{{Func5|UIManager|SetUICursor}}<b>(</b>{{Type5|PolicyBranchType}} oldCursor<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|PolicyBranchType]]
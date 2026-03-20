{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>AdvisorType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>AdvisorType</code> corresponds to the constants defined in the '''AdvisorTypes''' Lua enumeration.
}}


= Lua: the AdvisorTypes enumeration =
Firaxis provides a Lua enumeration named <code>AdvisorTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_ADVISOR_TYPE"
|
|align="right" |-1
|-
|align="left" |"ADVISOR_MILITARY"
|
|align="right" |0
|-
|align="left" |"ADVISOR_ECONOMIC"
|
|align="right" |1
|-
|align="left" |"ADVISOR_FOREIGN"
|
|align="right" |2
|-
|align="left" |"ADVISOR_SCIENCE"
|
|align="right" |3
|-
|align="left" |"NUM_ADVISOR_TYPES"
|
|align="right" |4
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = AdvisorTypes.ADVISOR_MILITARY
local id = AdvisorTypes["ADVISOR_MILITARY"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ISBUILDINGRECOMMENDED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsBuildingRecommended}}<b>(</b>'''int''' building, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
ISPROJECTRECOMMENDED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsProjectRecommended}}<b>(</b>'''int''' project, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
ISTECHRECOMMENDED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsTechRecommended}}<b>(</b>{{Type5|TechType}} arg0, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
ISUNITRECOMMENDED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsUnitRecommended}}<b>(</b>'''int''' unit, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|AdvisorType]]
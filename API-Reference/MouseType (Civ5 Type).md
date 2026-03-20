{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MouseType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>MouseType</code> corresponds to the constants defined in the '''Mouse''' Lua enumeration.
}}


= Lua: the Mouse enumeration =
Firaxis provides a Lua enumeration named <code>Mouse</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"eLClick"
|
|align="right" |0
|-
|align="left" |"eRClick"
|
|align="right" |1
|-
|align="left" |"eMClick"
|
|align="right" |2
|-
|align="left" |"eWheel"
|
|align="right" |3
|-
|align="left" |"eMouseEnter"
|
|align="right" |4
|-
|align="left" |"eMouseExit"
|
|align="right" |5
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = Mouse.eLClick
local id = Mouse["eLClick"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|BoxButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b><b>)</b>) MPListEntryClick<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Button}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} lClick, ('''void''' func<b>(</b>{{Type5|HandicapType}} index, {{Type5|ResourceType}} y, {{Type5|Button}} button, '''int''' x, '''int''' y<b>)</b>) OnEndTurnTimerClicked<b>)</b></code>
<!-- 
CLEARCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>ButtonBase:{{Func5|UIElement|ClearCallback}}<b>(</b>{{Type5|MouseType}} arg0<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|CheckBox}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|SpecialistType}} Inc<b>)</b>) ModUnitFort<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Grid}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} thisEvent, ('''void''' func<b>(</b>{{Type5|PlayerID}} void1, {{Type5|ResourceType}} void2, {{Type5|Button}} button<b>)</b>) OnContinueButtonClicked<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GridButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|PolicyType}} Id, {{Type5|ResourceType}} none, {{Type5|Button}} control<b>)</b>) OnEndTurnClicked<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Image}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|EndTurnBlockingType}} Id<b>)</b>) OnEditNameClick<b>)</b></code>
<!-- 
ADVISORBUTTONEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|LuaEvents}}.{{Func5|LuaEvents|AdvisorButtonEvent}}<b>(</b>{{Type5|MouseType}} button<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|RadioButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|SpecialistType}} void1, '''int''' Control<b>)</b>) ModeClicked<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Stack}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|EndTurnBlockingType}} Id<b>)</b>) GenericLeftClick<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TextButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|SpecialistType}} ePlayer<b>)</b>) OnCancelEditPlayerDetails<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TextButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} OnSearchTextEnter, ('''void''' func<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex, {{Type5|UnitType}} y, {{Type5|Button}} button<b>)</b>) OnClose = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MouseType]]
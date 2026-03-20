{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>InterfaceDirtyBits</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{Lua}} Integers labeled as <code>InterfaceDirtyBits</code> corresponds to the constants defined in the '''InterfaceDirtyBits''' Lua enumeration.
}}


= Lua: the InterfaceDirtyBits enumeration =
Firaxis provides a Lua enumeration named <code>InterfaceDirtyBits</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"SelectionCamera_DIRTY_BIT"
|
|align="right" |0
|-
|align="left" |"Fog_DIRTY_BIT"
|
|align="right" |1
|-
|align="left" |"Waypoints_DIRTY_BIT"
|
|align="right" |2
|-
|align="left" |"PercentButtons_DIRTY_BIT"
|
|align="right" |3
|-
|align="left" |"MiscButtons_DIRTY_BIT"
|
|align="right" |4
|-
|align="left" |"PlotListButtons_DIRTY_BIT"
|
|align="right" |5
|-
|align="left" |"SelectionButtons_DIRTY_BIT"
|
|align="right" |6
|-
|align="left" |"CitizenButtons_DIRTY_BIT"
|
|align="right" |7
|-
|align="left" |"ResearchButtons_DIRTY_BIT"
|
|align="right" |8
|-
|align="left" |"Event_DIRTY_BIT"
|
|align="right" |9
|-
|align="left" |"Center_DIRTY_BIT"
|
|align="right" |10
|-
|align="left" |"GameData_DIRTY_BIT"
|
|align="right" |11
|-
|align="left" |"Score_DIRTY_BIT"
|
|align="right" |12
|-
|align="left" |"TurnTimer_DIRTY_BIT"
|
|align="right" |13
|-
|align="left" |"Help_DIRTY_BIT"
|
|align="right" |14
|-
|align="left" |"MinimapSection_DIRTY_BIT"
|
|align="right" |15
|-
|align="left" |"SelectionSound_DIRTY_BIT"
|
|align="right" |16
|-
|align="left" |"Cursor_DIRTY_BIT"
|
|align="right" |17
|-
|align="left" |"CityInfo_DIRTY_BIT"
|
|align="right" |18
|-
|align="left" |"UnitInfo_DIRTY_BIT"
|
|align="right" |19
|-
|align="left" |"Popup_DIRTY_BIT"
|
|align="right" |20
|-
|align="left" |"CityScreen_DIRTY_BIT"
|
|align="right" |21
|-
|align="left" |"InfoPane_DIRTY_BIT"
|
|align="right" |22
|-
|align="left" |"HighlightPlot_DIRTY_BIT"
|
|align="right" |23
|-
|align="left" |"ColoredPlots_DIRTY_BIT"
|
|align="right" |24
|-
|align="left" |"BlockadedPlots_DIRTY_BIT"
|
|align="right" |25
|-
|align="left" |"Financial_Screen_DIRTY_BIT"
|
|align="right" |26
|-
|align="left" |"Foreign_Screen_DIRTY_BIT"
|
|align="right" |27
|-
|align="left" |"Soundtrack_DIRTY_BIT"
|
|align="right" |28
|-
|align="left" |"Domestic_Advisor_DIRTY_BIT"
|
|align="right" |29
|-
|align="left" |"Advanced_Start_DIRTY_BIT"
|
|align="right" |30
|-
|align="left" |"NationalBorders_DIRTY_BIT"
|
|align="right" |31
|-
|align="left" |"Policies_DIRTY_BIT"
|
|align="right" |32
|-
|align="left" |"PlotData_DIRTY_BIT"
|
|align="right" |33
|-
|align="left" |"NUM_INTERFACE_DIRTY_BITS"
|
|align="right" |35
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = InterfaceDirtyBits.SelectionCamera_DIRTY_BIT
local id = InterfaceDirtyBits["SelectionCamera_DIRTY_BIT"]
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
SETDIRTY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SetDirty}}<b>(</b>{{Type5|InterfaceDirtyBits}} arg0, '''bool''' arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|InterfaceDirtyBits]]
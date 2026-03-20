{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>HandicapType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>HandicapType</code> corresponds to the ''ID'' column of the {{Table5|HandicapInfos|CIV5HandicapInfos}} XML table.
}}


= XML: the HandicapInfos table =
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
|HANDICAP_SETTLER
|-
|align="right"|1
|
|HANDICAP_CHIEFTAIN
|-
|align="right"|2
|
|HANDICAP_WARLORD
|-
|align="right"|3
|
|HANDICAP_PRINCE
|-
|align="right"|4
|
|HANDICAP_KING
|-
|align="right"|5
|
|HANDICAP_EMPEROR
|-
|align="right"|6
|
|HANDICAP_IMMORTAL
|-
|align="right"|7
|
|HANDICAP_DEITY
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Button}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} lClick, ('''void''' func<b>(</b>{{Type5|HandicapType}} index, {{Type5|ResourceType}} y, {{Type5|Button}} button, '''int''' x, '''int''' y<b>)</b>) OnEndTurnTimerClicked<b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SERIALEVENTUNITFLAGSELECTED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventUnitFlagSelected}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|HandicapType}} unit<b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAP
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetHandicap}}<b>(</b>{{Type5|PlayerID}} player = nil<b>)</b></code>
<!-- 
GETWORLDSIZE
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetWorldSize}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETHANDICAP
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetHandicap}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|HandicapType}} id<b>)</b></code>
<!-- 
SETWORLDSIZE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetWorldSize}}<b>(</b>{{Type5|HandicapType}} id<b>)</b></code>
<!-- 
REGISTERSELECTIONCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PullDown}}:{{Func5|UIElement|RegisterSelectionCallback}}<b>(</b>('''void''' func<b>(</b>{{Type5|PlayerID}} playerID, {{Type5|HandicapType}} id, '''unknown''' control<b>)</b>) OnChatTarget<b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAPTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|HandicapType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetHandicapType}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|HandicapType]]
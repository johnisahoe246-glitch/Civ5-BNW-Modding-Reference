{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>GameSpeedType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>GameSpeedType</code> corresponds to the ''ID'' column of the {{Table5|GameSpeeds|CIV5GameSpeeds}} XML table.
}}


= XML: the GameSpeeds table =
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
|GAMESPEED_MARATHON
|-
|align="right"|1
|
|GAMESPEED_EPIC
|-
|align="right"|2
|
|GAMESPEED_STANDARD
|-
|align="right"|3
|
|GAMESPEED_QUICK
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETGAMESPEEDTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|GameSpeedType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetGameSpeedType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMESPEED
-->
|-
|align="right" width="200" |<code>{{Type5|GameSpeedType}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetGameSpeed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETGAMESPEED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|SetGameSpeed}}<b>(</b>{{Type5|GameSpeedType}} id<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameSpeedType]]
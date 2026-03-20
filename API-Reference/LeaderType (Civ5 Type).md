{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>LeaderType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>LeaderType</code> corresponds to the ''ID'' column of the {{Table5|Civilization_Leaders|CIV5Civilizations}} XML table.
}}


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETPERSONALITYTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|LeaderType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetPersonalityType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDPLAYER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|AddPlayer}}<b>(</b>{{Type5|PlayerID}} newPlayer, {{Type5|LeaderType}} leader, {{Type5|CivilizationType}} civ<b>)</b></code>
<!-- 
ISLEADEREVERACTIVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsLeaderEverActive}}<b>(</b>{{Type5|LeaderType}} leader<b>)</b></code>
<!-- 
GETLEADERTYPE
-->
|-
|align="right" width="200" |<code>{{Type5|LeaderType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetLeaderType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLEADERTYPE
-->
|-
|align="right" width="200" |<code>{{UnknownSignature5}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetLeaderType}}<!-- No arguments --></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|LeaderType]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|ActivePlayer}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|Calendar}}
:Type: {{Type5|CalendarType}}
:Usage: Unknown.

{{PseudoH4|Era}}
:Type: {{Type5|EraType}}
:Usage: Unknown.

{{PseudoH4|FinalTurn}}
:Type: {{Type5|PlayerID}}
:Usage: Unknown.

{{PseudoH4|GameSpeed}}
:Type: {{Type5|GameSpeedType}}
:Usage: Unknown.

{{PseudoH4|InitialTurn}}
:Type: {{Type5|PlayerID}}
:Usage: Unknown.

{{PseudoH4|MapHeight}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|MapWidth}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|Messages}}
:Type: table('''int''' => '''table''')
:Usage: Unknown.

{{PseudoH4|PlayerInfo}}
:Type: table('''int''' => '''table''')
:Usage: Unknown.

{{PseudoH4|Plots}}
:Type: table('''int''' => table({{Type5|PlayerID}} => '''table'''))
:Usage: Unknown.

{{PseudoH4|StartYear}}
:Type: '''int'''
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETREPLAYINFO
-->
|-
|align="right" width="200" |<code>{{Type5|ReplayInfo}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetReplayInfo}}<b>(</b>'''string''' file<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ReplayInfo]]
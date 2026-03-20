{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|DiscoveringPlayer}}
:Type: {{Type5|PlayerID}}
:Usage: Unknown.

{{PseudoH4|Plots}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|SpyName}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|String}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|Text}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|Turn}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|Type}}
:Type: '''unknown'''
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETREPLAYMESSAGES
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|IntrigueInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetReplayMessages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINTRIGUEMESSAGES
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|IntrigueInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetIntrigueMessages}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|IntrigueInfo]]
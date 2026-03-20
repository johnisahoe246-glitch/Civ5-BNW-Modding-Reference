{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|hostedDLC}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|MapName}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|maxPlayers}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|numPlayers}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|Players}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|requiredDLCAvailable}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|serverID}}
:Type: {{Type5|PlayerID}}
:Usage: Unknown.

{{PseudoH4|serverName}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|WorldSize}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|WorldSizeTranslated}}
:Type: '''unknown'''
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETMULTIPLAYERGAMELIST
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|MultiplayerGame}})</code>
|style="padding-left:6px" |<code>{{Type5|Matchmaking}}.{{Func5|Matchmaking|GetMultiplayerGameList}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MultiplayerGame]]
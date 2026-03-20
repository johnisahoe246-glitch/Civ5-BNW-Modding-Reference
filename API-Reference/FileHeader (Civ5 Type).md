{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|CivilizationName}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|CurrentEra}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|Difficulty}}
:Type: {{Type5|HandicapType}}
:Usage: Unknown.

{{PseudoH4|GameSpeed}}
:Type: {{Type5|GameSpeedType}}
:Usage: Unknown.

{{PseudoH4|GameType}}
:Type: {{Type5|GameType}}
:Usage: Unknown.

{{PseudoH4|LeaderName}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|MapScript}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|PlayerCivilization}}
:Type: {{Type5|CivilizationType}}
:Usage: Unknown.

{{PseudoH4|StartEra}}
:Type: {{Type5|EraType}}
:Usage: Unknown.

{{PseudoH4|TurnNumber}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|WorldSize}}
:Type: {{Type5|HandicapType}}
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETFILEHEADER
-->
|-
|align="right" width="200" |<code>{{Type5|FileHeader}}</code>
|style="padding-left:6px" |<code>{{Type5|PreGame}}.{{Func5|PreGame|GetFileHeader}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
GETCLOUDSAVES
-->
|-
|align="right" width="200" |<code>table({{Type5|SpecialistType}} => {{Type5|FileHeader}})</code>
|style="padding-left:6px" |<code>{{Type5|Steam}}.{{Func5|Steam|GetCloudSaves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREPLAYFILEHEADER
-->
|-
|align="right" width="200" |<code>{{Type5|FileHeader}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetReplayFileHeader}}<b>(</b>'''unknown''' arg0<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|FileHeader]]
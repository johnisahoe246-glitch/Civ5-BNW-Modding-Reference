{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|BasePotential}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|CityID}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|CityX}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|CityY}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|Civilization}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|CivilizationIconAtlas}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|CivilizationIconColor}}
:Type: {{Type5|Vector4}}
:Usage: Unknown.

{{PseudoH4|CivilizationName}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|CivilizationNameKey}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|CivilizationPortraitIndex}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|LargestBasePotential}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|Name}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|PlayerID}}
:Type: {{Type5|PlayerID}}
:Usage: Unknown.

{{PseudoH4|Population}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|Potential}}
:Type: '''int'''
:Usage: Unknown.

{{PseudoH4|Team}}
:Type: {{Type5|TeamID}}
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETESPIONAGECITYSTATUS
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|CityEspionageInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetEspionageCityStatus}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CityEspionageInfo]]
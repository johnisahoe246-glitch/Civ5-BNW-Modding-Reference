{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|MaxVersion}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|MinVersion}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|ModID}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|PackageID}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|Type}}
:Type: '''int'''
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETDLCASSOCIATIONS
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|ModDependency}})</code>
|style="padding-left:6px" |<code>{{Type5|Modding}}.{{Func5|Modding|GetDlcAssociations}}<b>(</b>'''string''' modId, '''int''' modVersion<b>)</b></code>
<!-- 
GETGAMEVERSIONASSOCIATIONS
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|ModDependency}})</code>
|style="padding-left:6px" |<code>{{Type5|Modding}}.{{Func5|Modding|GetGameVersionAssociations}}<b>(</b>'''string''' modId, '''int''' modVersion<b>)</b></code>
<!-- 
GETMODASSOCIATIONS
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|ModDependency}})</code>
|style="padding-left:6px" |<code>{{Type5|Modding}}.{{Func5|Modding|GetModAssociations}}<b>(</b>'''string''' modId, '''int''' modVersion<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ModDependency]]
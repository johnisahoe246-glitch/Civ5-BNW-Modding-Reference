{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|DisplayName}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|DownloadHandle}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|Enabled}}
:Type: '''bool'''
:Usage: Unknown.

{{PseudoH4|ModId}}
:Type: {{Type5|Button}}
:Usage: Unknown.

{{PseudoH4|Name}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|PublishedFileId}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|State}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|Teaser}}
:Type: '''string'''
:Usage: Unknown.

{{PseudoH4|Title}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|Type}}
:Type: '''unknown'''
:Usage: Unknown.

{{PseudoH4|Version}}
:Type: {{Type5|Button}}
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCURRENTLANGUAGE
-->
|-
|align="right" width="200" |<code>{{Type5|ModInfo}}</code>
|style="padding-left:6px" |<code>{{Type5|Locale}}.{{Func5|Locale|GetCurrentLanguage}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRENTSPOKENLANGUAGE
-->
|-
|align="right" width="200" |<code>{{Type5|ModInfo}}</code>
|style="padding-left:6px" |<code>{{Type5|Locale}}.{{Func5|Locale|GetCurrentSpokenLanguage}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSUPPORTEDLANGUAGES
-->
|-
|align="right" width="200" |<code>table({{Type5|EraType}} => {{Type5|ModInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Locale}}.{{Func5|Locale|GetSupportedLanguages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSUPPORTEDSPOKENLANGUAGES
-->
|-
|align="right" width="200" |<code>table({{Type5|EraType}} => {{Type5|ModInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Locale}}.{{Func5|Locale|GetSupportedSpokenLanguages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMODBROWSERDOWNLOADINGLISTINGS
-->
|-
|align="right" width="200" |<code>table('''int''' => {{Type5|ModInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Modding}}.{{Func5|Modding|GetModBrowserDownloadingListings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMODBROWSERINSTALLEDLISTINGS
-->
|-
|align="right" width="200" |<code>table('''string''' => {{Type5|ModInfo}})</code>
|style="padding-left:6px" |<code>{{Type5|Modding}}.{{Func5|Modding|GetModBrowserInstalledListings}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ModInfo]]
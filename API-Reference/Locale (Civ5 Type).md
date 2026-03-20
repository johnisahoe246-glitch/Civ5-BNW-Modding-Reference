{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Locale.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
COMPARE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|Compare}}<b>(</b>'''string''' a, '''string''' b<b>)</b></code>
<!-- 
CONVERTTEXTKEY
-->
|-
{{FuncInfos5|yes  |yes  |yes|Converts a text key into a localized string}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|ConvertTextKey}}<b>(</b>'''string''' key, ...<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ENDSWITH
-->
|-
{{FuncInfos5|yes  |yes  |yes|Test if a string ends with a specified suffix (UTF-8 friendly)}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|EndsWith}}<b>(</b>'''string''' base_string, '''string''' suffix<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCURRENTLANGUAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ModInfo}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|GetCurrentLanguage}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRENTSPOKENLANGUAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ModInfo}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|GetCurrentSpokenLanguage}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHOTKEYDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |yes|Returns a localized description for a hotkey}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|GetHotKeyDescription}}<b>(</b>'''string''' key, '''bool''' ctrl = nil, '''bool''' alt = nil, '''bool''' shift = nil<b>)</b></code>
<!-- 
GETSUPPORTEDLANGUAGES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table({{Type5|EraType}} => {{Type5|ModInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Locale|GetSupportedLanguages}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSUPPORTEDSPOKENLANGUAGES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table({{Type5|EraType}} => {{Type5|ModInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Locale|GetSupportedSpokenLanguages}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASTEXTKEY
-->
|-
{{FuncInfos5|yes  |yes  |yes|Determine if a textkey can be found in the Localization System's string dictionary}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|HasTextKey}}<b>(</b>'''string''' textkey<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISASCII
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|IsASCII}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISNILOREMPTY
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|IsNilOrEmpty}}<b>(</b>'''string''' name<b>)</b></code>
<!-- 
ISNILORWHITESPACE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|IsNilOrWhitespace}}<b>(</b>'''int''' name<b>)</b></code>
<!-- 
ISUTF8
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|IsUTF8}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==L==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
LENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|Length}}<b>(</b>'''string''' info<b>)</b></code>
<!-- 
LOCALSYSTEMCPTOUTF8
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|LocalSystemCPToUTF8}}<!-- No arguments --></code>
<!-- 
LOOKUP
-->
|-
{{FuncInfos5|yes  |yes  |yes|Converts a text key into a localized string}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|Lookup}}<b>(</b>'''string''' key, ...<b>)</b></code>
<!-- 
LOOKUPLANGUAGE
-->
|-
{{FuncInfos5|yes  |yes  |yes|Lookup a textkey using another language as the primary language}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|LookupLanguage}}<b>(</b>'''string''' language, '''string''' key, ...<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETCURRENTLANGUAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Locale|SetCurrentLanguage}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
SETCURRENTSPOKENLANGUAGE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Locale|SetCurrentSpokenLanguage}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
STARTSWITH
-->
|-
{{FuncInfos5|maybe|maybe|yes|Test if a string starts with a specified prefix (UTF-8 friendly)}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|StartsWith}}<b>(</b>'''string''' base_string, '''string''' prefix<b>)</b></code>
<!-- 
SUBSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|Substring}}<b>(</b>'''string''' info, '''int''' arg1, '''int''' newLength<b>)</b></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TOCURRENCY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|ToCurrency}}<!-- No arguments --></code>
<!-- 
TOLOWER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|ToLower}}<b>(</b>'''string''' name<b>)</b></code>
<!-- 
TONUMBER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|ToNumber}}<b>(</b>'''int''' netGPT, '''string''' arg1<b>)</b></code>
<!-- 
TOPERCENT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|ToPercent}}<!-- No arguments --></code>
<!-- 
TOROMANNUMERAL
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|ToRomanNumeral}}<!-- No arguments --></code>
<!-- 
TOSPELLOUT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|ToSpellout}}<!-- No arguments --></code>
<!-- 
TOUPPER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|ToUpper}}<b>(</b>'''string''' localizedCityName<b>)</b></code>
<!-- 
TRUNCATESTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Locale|TruncateString}}<b>(</b>'''string''' title, '''int''' maxTechNameLength, '''bool''' arg2<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UTF8TOLOCALSYSTEMCP
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Locale|UTF8ToLocalSystemCP}}<!-- No arguments --></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Locale]]
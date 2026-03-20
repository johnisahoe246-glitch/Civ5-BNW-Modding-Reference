{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>ContentManager.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETALLPACKAGEIDS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|ContentManager|GetAllPackageIDs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPACKAGEDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|ContentManager|GetPackageDescription}}<b>(</b>'''unknown''' v<b>)</b></code>
<!-- 
ISACTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|ContentManager|IsActive}}<b>(</b>'''string''' v, {{Type5|ContentType}} arg1<b>)</b></code>
<!-- 
SETACTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|ContentManager|SetActive}}<b>(</b>table('''int''' => table('''int''' => '''string''')) packages<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ContentManager]]
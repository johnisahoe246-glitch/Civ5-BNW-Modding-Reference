{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This object is defined in the following Lua source file: ''TerrainGenerator.lua''.
:To import it, use: <code>include("TerrainGenerator")</code>}}


=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>TerrainGenerator.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CREATE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|TerrainGenerator|Create}}<b>(</b>'''table''' args<b>)</b></code>
|}


=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of TerrainGenerator.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GENERATETERRAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|TerrainType}})</code>
|width="100%" |<code>{{FuncLabel5|TerrainGenerator|GenerateTerrain}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATETERRAINATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TerrainGenerator|GenerateTerrainAtPlot}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
GETLATITUDEATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TerrainGenerator|GetLatitudeAtPlot}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
INITFRACTALS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TerrainGenerator|InitFractals}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|TerrainGenerator]]
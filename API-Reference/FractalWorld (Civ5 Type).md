{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This object is defined in the following Lua source file: ''FractalWorld.lua''.
:To import it, use: <code>include("FractalWorld")</code>}}


=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>FractalWorld.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CREATE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|Create}}<b>(</b>'''float''' fracXExp = nil, '''float''' fracYExp = nil<b>)</b></code>
|}


=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of FractalWorld.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DETERMINEXSHIFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|DetermineXShift}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DETERMINEYSHIFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|DetermineYShift}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATECENTERRIFT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|GenerateCenterRift}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATEPLOTTYPES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|GeneratePlotTypes}}<b>(</b>'''int''' args<b>)</b></code>
<!-- 
INITFRACTAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|InitFractal}}<b>(</b>'''table''' args<b>)</b></code>
<!-- 
SHIFTPLOTTYPES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|ShiftPlotTypes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SHIFTPLOTTYPESBY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FractalWorld|ShiftPlotTypesBy}}<b>(</b>'''int''' xshift, '''int''' yshift<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|FractalWorld]]
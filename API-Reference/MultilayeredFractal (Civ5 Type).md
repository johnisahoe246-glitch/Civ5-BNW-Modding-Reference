{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This object is defined in the following Lua source file: ''Europe.lua''.
:To import it, use: <code>include("Europe")</code>}}


=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>MultilayeredFractal.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CREATE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|Create}}<b>(</b><!-- No arguments --><b>)</b></code>
|}


=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of MultilayeredFractal.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
APPLYTECTONICS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|ApplyTectonics}}<b>(</b>'''int''' args<b>)</b></code>
<!-- 
DETERMINEXSHIFT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|DetermineXShift}}<b>(</b>'''int''' regionWidth, '''int''' regionHeight<b>)</b></code>
<!-- 
DETERMINEYSHIFT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|DetermineYShift}}<b>(</b>'''int''' regionWidth, '''int''' regionHeight<b>)</b></code>
<!-- 
GENERATEFRACTALLAYER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|GenerateFractalLayer}}<b>(</b>'''int''' args<b>)</b></code>
<!-- 
GENERATEFRACTALLAYERWITHOUTHILLS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|GenerateFractalLayerWithoutHills}}<b>(</b>'''int''' args<b>)</b></code>
<!-- 
GENERATEPLOTSBYREGION
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|GeneratePlotsByRegion}}<!-- No arguments --></code>
<!-- 
GENERATEWATERLAYER
-->
|-
{{FuncInfos5|maybe|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|GenerateWaterLayer}}<b>(</b>'''int''' args<b>)</b></code>
<!-- 
SHIFTREGIONPLOTS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|ShiftRegionPlots}}<b>(</b>'''int''' regionWidth, '''int''' regionHeight<b>)</b></code>
<!-- 
SHIFTREGIONPLOTSBY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|MultilayeredFractal|ShiftRegionPlotsBy}}<b>(</b>'''int''' xshift, '''int''' yshift, '''int''' regionWidth, '''int''' regionHeight<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MultilayeredFractal]]
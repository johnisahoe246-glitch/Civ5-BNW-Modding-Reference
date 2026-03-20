{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Fractal.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CREATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Fractal}}</code>
|width="100%" |<code>{{FuncLabel5|Fractal|Create}}<b>(</b>'''int''' width, '''int''' height, '''int''' grain, '''int''' fractalFlags, '''float''' xExponent, '''float''' yExponent<b>)</b></code>
<!-- 
CREATERIFTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Fractal}}</code>
|width="100%" |<code>{{FuncLabel5|Fractal|CreateRifts}}<b>(</b>'''int''' regionWidth, '''int''' regionHeight, '''int''' continent_grain, '''table''' fracFlags, {{Type5|Fractal}} riftsFrac, '''float''' regionFracXExp, '''float''' regionFracYExp<b>)</b></code>
|}


=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Fractal.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
BUILDRIDGES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Fractal|BuildRidges}}<b>(</b>'''int''' numPlates, '''table''' flags, '''int''' xExponent, '''int''' yExponent<b>)</b></code>
<!-- 
GETHEIGHT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Fractal|GetHeight}}<b>(</b>'''int''' x, '''int''' y = nil<b>)</b></code>
|}

=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CREATE
-->
|-
|align="right" width="200" |<code>{{Type5|Fractal}}</code>
|style="padding-left:6px" |<code>{{Type5|Fractal}}.{{Func5|Fractal|Create}}<b>(</b>'''int''' width, '''int''' height, '''int''' grain, '''int''' fractalFlags, '''float''' xExponent, '''float''' yExponent<b>)</b></code>
<!-- 
CREATERIFTS
-->
|-
|align="right" width="200" |<code>{{Type5|Fractal}}</code>
|style="padding-left:6px" |<code>{{Type5|Fractal}}.{{Func5|Fractal|CreateRifts}}<b>(</b>'''int''' regionWidth, '''int''' regionHeight, '''int''' continent_grain, '''table''' fracFlags, {{Type5|Fractal}} riftsFrac, '''float''' regionFracXExp, '''float''' regionFracYExp<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Fractal]]
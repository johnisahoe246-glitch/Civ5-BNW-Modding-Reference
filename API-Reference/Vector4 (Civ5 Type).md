{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|w}}
:Type: '''float'''
:Usage: Unknown.

{{PseudoH4|x}}
:Type: '''float'''
:Usage: Unknown.

{{PseudoH4|y}}
:Type: '''float'''
:Usage: Unknown.

{{PseudoH4|z}}
:Type: '''float'''
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
COLOR
-->
|-
|align="right" width="200" |<code>{{Type5|Vector4}}</code>
|style="padding-left:6px" |<code>{{Func5|Color}}<b>(</b>'''float''' r, '''float''' g, '''float''' b, '''float''' a<b>)</b></code>
<!-- 
VECTOR4
-->
|-
|align="right" width="200" |<code>{{Type5|Vector4}}</code>
|style="padding-left:6px" |<code>{{Func5|Vector4}}<b>(</b>'''float''' i, '''float''' j = nil, '''float''' k = nil, '''float''' l = nil<b>)</b></code>
<!-- 
SETFGCOLOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Bar}}:{{Func5|UIElement|SetFGColor}}<b>(</b>{{Type5|Vector4}} tBarColor<b>)</b></code>
<!-- 
SERIALEVENTHEXHIGHLIGHT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventHexHighlight}}<b>(</b>{{Type5|Vector2}} hex, '''bool''' highlight, {{Type5|Vector4}} highlightColor, '''string''' highlightStyle<b>)</b></code>
<!-- 
SETCOLOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Image}}:{{Func5|UIElement|SetColor}}<b>(</b>{{Type5|Vector4}} primaryColorVector<b>)</b></code>
<!-- 
SETCOLOR
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Label}}:{{Func5|UIElement|SetColor}}<b>(</b>{{Type5|Vector4}} textColor200, '''int''' arg1<b>)</b></code>
<!-- 
GETPLAYERCOLORS
-->
|-
|align="right" width="200" |<code>{{Type5|Vector4}}, {{Type5|Vector4}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPlayerColors}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Vector4]]
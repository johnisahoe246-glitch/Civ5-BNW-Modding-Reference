{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This pseudo-type is a regular Lua table. You can create one manually by defining the same fields as the ones described below.}}


=Fields=
{{PseudoH4|x}}
:Type: '''float'''
:Usage: Unknown.

{{PseudoH4|y}}
:Type: '''float'''
:Usage: Unknown.


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
HEXTOWORLD
-->
|-
|align="right" width="200" |<code>{{Type5|Vector3}}</code>
|style="padding-left:6px" |<code>{{Func5|HexToWorld}}<b>(</b>{{Type5|Vector2}} hexPos<b>)</b></code>
<!-- 
ICONLOOKUP
-->
|-
|align="right" width="200" |<code>{{Type5|Vector2}}, '''string'''</code>
|style="padding-left:6px" |<code>{{Func5|IconLookup}}<b>(</b>'''int''' offset, '''int''' iconSize, '''string''' atlas<b>)</b></code>
<!-- 
TOHEXFROMGRID
-->
|-
|align="right" width="200" |<code>{{Type5|Vector2}}</code>
|style="padding-left:6px" |<code>{{Func5|ToHexFromGrid}}<b>(</b>{{Type5|Vector2}} gridPos<b>)</b></code>
<!-- 
VECTOR2
-->
|-
|align="right" width="200" |<code>{{Type5|Vector2}}</code>
|style="padding-left:6px" |<code>{{Func5|Vector2}}<b>(</b>'''float''' i, '''float''' j<b>)</b></code>
<!-- 
SETTEXTUREOFFSET
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Context}}:{{Func5|UIElement|SetTextureOffset}}<b>(</b>{{Type5|Vector2}} questionOffset<b>)</b></code>
<!-- 
SETOFFSET
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>ControlBase:{{Func5|UIElement|SetOffset}}<b>(</b>{{Type5|Vector2}} offset<b>)</b></code>
<!-- 
HEXFOWSTATECHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|HexFOWStateChanged}}<b>(</b>{{Type5|Vector2}} hexPos, '''int''' fowType, '''bool''' wholeMap<b>)</b></code>
<!-- 
SERIALEVENTCAMERAIN
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCameraIn}}<b>(</b>{{Type5|Vector2}} arg0<b>)</b></code>
<!-- 
SERIALEVENTCAMERAOUT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCameraOut}}<b>(</b>{{Type5|Vector2}} arg0<b>)</b></code>
<!-- 
SERIALEVENTCITYCAPTURED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityCaptured}}<b>(</b>{{Type5|Vector2}} hexPos, {{Type5|PlayerID}} player, '''int''' cityID, {{Type5|PlayerID}} newPlayer<b>)</b></code>
<!-- 
SERIALEVENTCITYCREATED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityCreated}}<b>(</b>{{Type5|Vector2}} vHexPos, {{Type5|PlayerID}} player, {{Type5|CityID}} cityID, {{Type5|ArtStyleType}} artStyleType, {{Type5|EraType}} eraType, '''int''' continent, '''int''' populationSize, '''int''' size, '''int''' fogState<b>)</b></code>
<!-- 
SERIALEVENTCITYDESTROYED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventCityDestroyed}}<b>(</b>{{Type5|Vector2}} hexPos, {{Type5|PlayerID}} player, '''int''' cityID, {{Type5|PlayerID}} newPlayer<b>)</b></code>
<!-- 
SERIALEVENTHEXHIGHLIGHT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|SerialEventHexHighlight}}<b>(</b>{{Type5|Vector2}} hex, '''bool''' highlight, {{Type5|Vector4}} highlightColor, '''string''' highlightStyle<b>)</b></code>
<!-- 
GETSIZE
-->
|-
|align="right" width="200" |<code>{{Type5|Vector2}}</code>
|style="padding-left:6px" |<code>{{Type5|Image}}:{{Func5|UIElement|GetSize}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETSIZE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Image}}:{{Func5|UIElement|SetSize}}<b>(</b>{{Type5|Vector2}} panelSize<b>)</b></code>
<!-- 
SETTEXTUREOFFSET
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Image}}:{{Func5|UIElement|SetTextureOffset}}<b>(</b>{{Type5|Vector2}} textureOffset<b>)</b></code>
<!-- 
SETTEXTUREOFFSET
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Stack}}:{{Func5|UIElement|SetTextureOffset}}<b>(</b>{{Type5|Vector2}} questionOffset<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Vector2]]
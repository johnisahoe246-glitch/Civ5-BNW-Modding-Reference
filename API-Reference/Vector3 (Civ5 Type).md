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

{{PseudoH4|z}}
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
VECTOR3
-->
|-
|align="right" width="200" |<code>{{Type5|Vector3}}</code>
|style="padding-left:6px" |<code>{{Func5|Vector3}}<b>(</b>'''float''' i, '''float''' j, '''float''' k<b>)</b></code>
<!-- 
ADDPOPUPTEXTEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|AddPopupTextEvent}}<b>(</b>{{Type5|Vector3}} worldPosition, '''unknown''' text, '''int''' delay<b>)</b></code>
<!-- 
LOCALMACHINEUNITPOSITIONCHANGED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|LocalMachineUnitPositionChanged}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, {{Type5|Vector3}} unitPosition<b>)</b></code>
<!-- 
SETWORLDPOSITION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|WorldAnchor}}:{{Func5|UIElement|SetWorldPosition}}<b>(</b>{{Type5|Vector3}} worldPos<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Vector3]]
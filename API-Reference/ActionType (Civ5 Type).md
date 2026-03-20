{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ActionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ActionType</code> corresponds to the ''ID'' column of the {{Table5|Commands|CIV5Commands}} XML table.
}}


= XML: the Commands table =
Here are the ''ID'' and ''Type'' columns found in this table.
<code>
{|
|-
!align="left" |ID
!
!align="left" |Type
|-
|align="right"|0
|
|COMMAND_PROMOTION
|-
|align="right"|1
|
|COMMAND_UPGRADE
|-
|align="right"|2
|
|COMMAND_AUTOMATE
|-
|align="right"|3
|
|COMMAND_WAKE
|-
|align="right"|4
|
|COMMAND_CANCEL
|-
|align="right"|5
|
|COMMAND_CANCEL_ALL
|-
|align="right"|6
|
|COMMAND_STOP_AUTOMATION
|-
|align="right"|7
|
|COMMAND_DELETE
|-
|align="right"|8
|
|COMMAND_GIFT
|-
|align="right"|9
|
|COMMAND_HOTKEY
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Commands.COMMAND_PROMOTION.ID
local id = GameInfo["Commands"].["COMMAND_PROMOTION"].ID
local id = GameInfo.Commands{Type="COMMAND_PROMOTION"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_COMMAND_PROMOTION.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Commands[0].Description
local description = GameInfo["Commands"][0]["Description"]
local description = GameInfo.Commands{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETVOLUMEKNOBIDFROMNAME
-->
|-
|align="right" width="200" |<code>{{Type5|ActionType}}</code>
|style="padding-left:6px" |<code>{{Func5|GetVolumeKnobIDFromName}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
GETVOLUMEKNOBVALUE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Func5|GetVolumeKnobValue}}<b>(</b>{{Type5|ActionType}} musicVolumeKnob<b>)</b></code>
<!-- 
SETVOLUMEKNOBVALUE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Func5|SetVolumeKnobValue}}<b>(</b>{{Type5|ActionType}} musicVolumeKnob, '''int''' cachedMusicVolumeKnob<b>)</b></code>
<!-- 
CANHANDLEACTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CanHandleAction}}<b>(</b>{{Type5|ActionType}} action, {{Type5|Plot}} plot = nil, '''bool''' testVisible = false<b>)</b></code>
<!-- 
GETVOID1
-->
|-
|align="right" width="200" |<code>{{Type5|ActionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Slider}}:{{Func5|UIElement|GetVoid1}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REGISTERSLIDERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Slider}}:{{Func5|UIElement|RegisterSliderCallback}}<b>(</b>('''void''' func<b>(</b>'''int''' fValue, {{Type5|ActionType}} void1<b>)</b>) OnMinorCivsSlider<b>)</b></code>
<!-- 
SETVOID1
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Slider}}:{{Func5|UIElement|SetVoid1}}<b>(</b>{{Type5|ActionType}} musicVolumeKnob<b>)</b></code>
<!-- 
ISACTIONRECOMMENDED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|IsActionRecommended}}<b>(</b>{{Type5|ActionType}} action<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ActionType]]
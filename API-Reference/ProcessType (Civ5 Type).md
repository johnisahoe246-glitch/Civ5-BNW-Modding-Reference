{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ProcessType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ProcessType</code> corresponds to the ''ID'' column of the {{Table5|Processes|CIV5Processes}} XML table.
}}


= XML: the Processes table =
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
|PROCESS_WEALTH
|-
|align="right"|1
|
|PROCESS_RESEARCH
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANMAINTAIN
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanMaintain}}<b>(</b>{{Type5|ProcessType}} process, '''int''' continue<b>)</b></code>
<!-- 
GETPRODUCTIONPROCESS
-->
|-
|align="right" width="200" |<code>{{Type5|ProcessType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProductionProcess}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETVOID2
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GridButton}}:{{Func5|UIElement|SetVoid2}}<b>(</b>{{Type5|ProcessType}} process<b>)</b></code>
<!-- 
CANMAINTAIN
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanMaintain}}<b>(</b>{{Type5|ProcessType}} process, '''bool''' continue<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ProcessType]]
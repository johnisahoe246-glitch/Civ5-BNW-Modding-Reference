{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>AutomateType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>AutomateType</code> corresponds to the ''ID'' column of the {{Table5|Automates|CIV5Automates}} XML table.
}}


= XML: the Automates table =
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
|AUTOMATE_BUILD
|-
|align="right"|1
|
|AUTOMATE_EXPLORE
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Automates.AUTOMATE_BUILD.ID
local id = GameInfo["Automates"].["AUTOMATE_BUILD"].ID
local id = GameInfo.Automates{Type="AUTOMATE_BUILD"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_ACTION_AUTOMATE_BUILD.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Automates[0].Description
local description = GameInfo["Automates"][0]["Description"]
local description = GameInfo.Automates{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANAUTOMATE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanAutomate}}<b>(</b>{{Type5|AutomateType}} automate<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|AutomateType]]
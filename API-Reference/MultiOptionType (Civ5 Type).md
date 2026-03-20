{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>MultiOptionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>MultiOptionType</code> corresponds to the ''ID'' column of the {{Table5|MultiplayerOptions|CIV5MultiplayerOptions}} XML table.
}}


= XML: the MultiplayerOptions table =
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
|MPOPTION_SIMULTANEOUS_TURNS
|-
|align="right"|1
|
|MPOPTION_TAKEOVER_AI
|-
|align="right"|2
|
|MPOPTION_SHUFFLE_TEAMS
|-
|align="right"|3
|
|MPOPTION_ANONYMOUS
|-
|align="right"|4
|
|MPOPTION_TURN_TIMER
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.MultiplayerOptions.MPOPTION_SIMULTANEOUS_TURNS.ID
local id = GameInfo["MultiplayerOptions"].["MPOPTION_SIMULTANEOUS_TURNS"].ID
local id = GameInfo.MultiplayerOptions{Type="MPOPTION_SIMULTANEOUS_TURNS"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_MP_OPTION_SIMULTANEOUS_TURNS.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.MultiplayerOptions[0].Description
local description = GameInfo["MultiplayerOptions"][0]["Description"]
local description = GameInfo.MultiplayerOptions{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ISMPOPTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsMPOption}}<b>(</b>{{Type5|MultiOptionType}} index<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|MultiOptionType]]
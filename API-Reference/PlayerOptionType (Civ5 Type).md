{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>PlayerOptionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>PlayerOptionType</code> corresponds to the ''ID'' column of the {{Table5|PlayerOptions|CIV5PlayerOptions}} XML table.
}}


= XML: the PlayerOptions table =
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
|PLAYEROPTION_WAIT_END_TURN
|-
|align="right"|1
|
|PLAYEROPTION_SHOW_FRIENDLY_MOVES
|-
|align="right"|2
|
|PLAYEROPTION_SHOW_ENEMY_MOVES
|-
|align="right"|3
|
|PLAYEROPTION_QUICK_MOVES
|-
|align="right"|4
|
|PLAYEROPTION_START_AUTOMATED
|-
|align="right"|5
|
|PLAYEROPTION_SAFE_AUTOMATION
|-
|align="right"|6
|
|PLAYEROPTION_NO_UNIT_CYCLING
|-
|align="right"|7
|
|PLAYEROPTION_LEAVE_FORESTS
|-
|align="right"|8
|
|PLAYEROPTION_MODDER_1
|-
|align="right"|9
|
|PLAYEROPTION_MODDER_2
|-
|align="right"|10
|
|PLAYEROPTION_MODDER_3
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.PlayerOptions.PLAYEROPTION_WAIT_END_TURN.ID
local id = GameInfo["PlayerOptions"].["PLAYEROPTION_WAIT_END_TURN"].ID
local id = GameInfo.PlayerOptions{Type="PLAYEROPTION_WAIT_END_TURN"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_PLAYER_OPTION_WAIT_AT_END_OF_TURN.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.PlayerOptions[0].Description
local description = GameInfo["PlayerOptions"][0]["Description"]
local description = GameInfo.PlayerOptions{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ISOPTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsOption}}<b>(</b>{{Type5|PlayerOptionType}} index<b>)</b></code>
<!-- 
SETOPTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetOption}}<b>(</b>{{Type5|PlayerOptionType}} index, '''bool''' newValue<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|PlayerOptionType]]
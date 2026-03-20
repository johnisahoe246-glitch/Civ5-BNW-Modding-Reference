{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>CalendarType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>CalendarType</code> corresponds to the ''ID'' column of the {{Table5|Calendars|CIV5Calendars}} XML table.
}}


= XML: the Calendars table =
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
|CALENDAR_DEFAULT
|-
|align="right"|1
|
|CALENDAR_BI_YEARLY
|-
|align="right"|2
|
|CALENDAR_YEARS
|-
|align="right"|3
|
|CALENDAR_TURNS
|-
|align="right"|4
|
|CALENDAR_SEASONS
|-
|align="right"|5
|
|CALENDAR_MONTHS
|-
|align="right"|6
|
|CALENDAR_WEEKS
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Calendars.CALENDAR_DEFAULT.ID
local id = GameInfo["Calendars"].["CALENDAR_DEFAULT"].ID
local id = GameInfo.Calendars{Type="CALENDAR_DEFAULT"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_CALENDAR_DEFAULT.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Calendars[0].Description
local description = GameInfo["Calendars"][0]["Description"]
local description = GameInfo.Calendars{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETCALENDAR
-->
|-
|align="right" width="200" |<code>{{Type5|CalendarType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetCalendar}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|CalendarType]]
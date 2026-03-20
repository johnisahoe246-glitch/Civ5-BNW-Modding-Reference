{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>InvisibilityScopeType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>InvisibilityScopeType</code> corresponds to the ''ID'' column of the {{Table5|InvisibleInfos|CIV5InvisibleInfos}} XML table.
}}


= XML: the InvisibleInfos table =
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
|INVISIBLE_SUBMARINE
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.InvisibleInfos.INVISIBLE_SUBMARINE.ID
local id = GameInfo["InvisibleInfos"].["INVISIBLE_SUBMARINE"].ID
local id = GameInfo.InvisibleInfos{Type="INVISIBLE_SUBMARINE"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_INVISIBLE_SUBMARINE.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.InvisibleInfos[0].Description
local description = GameInfo["InvisibleInfos"][0]["Description"]
local description = GameInfo.InvisibleInfos{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CHANGEINVISIBLEVISIBILITYCOUNT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|ChangeInvisibleVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible, '''int''' change<b>)</b></code>
<!-- 
CHANGEVISIBILITYCOUNT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|ChangeVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, '''int''' change, {{Type5|InvisibilityScopeType}} seeInvisibleType, '''bool''' informExplorationTracking, '''bool''' alwaysSeeInvisible<b>)</b></code>
<!-- 
GETINVISIBLEVISIBILITYCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetInvisibleVisibilityCount}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible<b>)</b></code>
<!-- 
ISINVISIBLEVISIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|IsInvisibleVisible}}<b>(</b>{{Type5|TeamID}} team, {{Type5|InvisibilityScopeType}} invisible<b>)</b></code>
<!-- 
GETINVISIBLETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|InvisibilityScopeType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetInvisibleType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSEEINVISIBLETYPE
-->
|-
|align="right" width="200" |<code>{{Type5|InvisibilityScopeType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetSeeInvisibleType}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|InvisibilityScopeType]]
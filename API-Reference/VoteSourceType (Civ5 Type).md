{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>VoteSourceType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>VoteSourceType</code> corresponds to the ''ID'' column of the {{Table5|VoteSources|CIV5VoteSources}} XML table.
}}


= XML: the VoteSources table =
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
|DIPLOVOTE_UN
|-
|align="right"|1
|
|DIPLOVOTE_POPE
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.VoteSources.DIPLOVOTE_UN.ID
local id = GameInfo["VoteSources"].["DIPLOVOTE_UN"].ID
local id = GameInfo.VoteSources{Type="DIPLOVOTE_UN"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_BUILDING_UNITED_NATIONS.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.VoteSources[0].Description
local description = GameInfo["VoteSources"][0]["Description"]
local description = GameInfo.VoteSources{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
CANHAVESECRETARYGENERAL
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CanHaveSecretaryGeneral}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
CHANGEDIPLOVOTE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|ChangeDiploVote}}<b>(</b>{{Type5|VoteSourceType}} voteSource, '''int''' change<b>)</b></code>
<!-- 
COUNTPOSSIBLEVOTE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CountPossibleVote}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETSECRETARYGENERAL
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetSecretaryGeneral}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETVOTEREQUIRED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetVoteRequired}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISDIPLOVOTE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsDiploVote}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISTEAMVOTEELIGIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsTeamVoteEligible}}<b>(</b>{{Type5|TeamID}} team, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETVOTES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetVotes}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISFULLMEMBER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsFullMember}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISVOTINGMEMBER
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsVotingMember}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
CHANGEFORCETEAMVOTEELIGIBILITYCOUNT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|ChangeForceTeamVoteEligibilityCount}}<b>(</b>{{Type5|VoteSourceType}} voteSource, '''int''' change<b>)</b></code>
<!-- 
GETFORCETEAMVOTEELIGIBILITYCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetForceTeamVoteEligibilityCount}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISFORCETEAMVOTEELIGIBLE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsForceTeamVoteEligible}}<b>(</b>{{Type5|VoteSourceType}} voteSource<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|VoteSourceType]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>VoteType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>VoteType</code> corresponds to the ''ID'' column of the {{Table5|Votes|CIV5Votes}} XML table.
}}


= XML: the Votes table =
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
|VOTE_SECRETARY_GENERAL
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Votes.VOTE_SECRETARY_GENERAL.ID
local id = GameInfo["Votes"].["VOTE_SECRETARY_GENERAL"].ID
local id = GameInfo.Votes{Type="VOTE_SECRETARY_GENERAL"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_VOTE_SECRETARY_GENERAL.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Votes[0].Description
local description = GameInfo["Votes"][0]["Description"]
local description = GameInfo.Votes{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
COUNTPOSSIBLEVOTE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CountPossibleVote}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
GETVOTEOUTCOME
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetVoteOutcome}}<b>(</b>{{Type5|VoteType}} index<b>)</b></code>
<!-- 
GETVOTEREQUIRED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetVoteRequired}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
<!-- 
ISCHOOSEELECTION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsChooseElection}}<b>(</b>{{Type5|VoteType}} vote<b>)</b></code>
<!-- 
ISTEAMVOTE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsTeamVote}}<b>(</b>{{Type5|VoteType}} vote<b>)</b></code>
<!-- 
ISVOTEPASSED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsVotePassed}}<b>(</b>{{Type5|VoteType}} index<b>)</b></code>
<!-- 
GETVOTES
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetVotes}}<b>(</b>{{Type5|VoteType}} vote, {{Type5|VoteSourceType}} voteSource<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|VoteType]]
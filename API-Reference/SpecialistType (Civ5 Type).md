{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>SpecialistType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>SpecialistType</code> corresponds to the ''ID'' column of the {{Table5|Specialists|CIV5Specialists}} XML table.
}}


= XML: the Specialists table =
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
|SPECIALIST_CITIZEN
|-
|align="right"|1
|
|SPECIALIST_ARTIST
|-
|align="right"|2
|
|SPECIALIST_SCIENTIST
|-
|align="right"|3
|
|SPECIALIST_MERCHANT
|-
|align="right"|4
|
|SPECIALIST_ENGINEER
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Specialists.SPECIALIST_CITIZEN.ID
local id = GameInfo["Specialists"].["SPECIALIST_CITIZEN"].ID
local id = GameInfo.Specialists{Type="SPECIALIST_CITIZEN"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_SPECIALIST_CITIZEN.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Specialists[0].Description
local description = GameInfo["Specialists"][0]["Description"]
local description = GameInfo.Specialists{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|CheckBox}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|SpecialistType}} Inc<b>)</b>) ModUnitFort<b>)</b></code>
<!-- 
CHANGESPECIALISTGREATPERSONPROGRESSTIMES100
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChangeSpecialistGreatPersonProgressTimes100}}<b>(</b>{{Type5|SpecialistType}} index, '''int''' change<b>)</b></code>
<!-- 
GETCULTUREFROMSPECIALIST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetCultureFromSpecialist}}<b>(</b>{{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETEXTRASPECIALISTYIELDOFTYPE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetExtraSpecialistYieldOfType}}<b>(</b>{{Type5|YieldType}} index, {{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETFIRSTSPECIALISTORDER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetFirstSpecialistOrder}}<b>(</b>{{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETPRODUCTIONSPECIALIST
-->
|-
|align="right" width="200" |<code>{{Type5|SpecialistType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProductionSpecialist}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSPECIALISTCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSpecialistCount}}<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>
<!-- 
GETSPECIALISTGREATPERSONPROGRESS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSpecialistGreatPersonProgress}}<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>
<!-- 
GETSPECIALISTGREATPERSONPROGRESSTIMES100
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSpecialistGreatPersonProgressTimes100}}<b>(</b>{{Type5|SpecialistType}} index<b>)</b></code>
<!-- 
GETSPECIALISTPRODUCTIONMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSpecialistProductionModifier}}<b>(</b>{{Type5|SpecialistType}} specialist<b>)</b></code>
<!-- 
GETSPECIALISTPRODUCTIONTURNSLEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSpecialistProductionTurnsLeft}}<b>(</b>{{Type5|SpecialistType}} specialist, '''int''' num<b>)</b></code>
<!-- 
GETSPECIALISTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetSpecialistYield}}<b>(</b>{{Type5|SpecialistType}} specialist, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
REMOVECITYTRADE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Deal}}:{{Func5|Deal|RemoveCityTrade}}<b>(</b>{{Type5|SpecialistType}} player, '''int''' cityID<b>)</b></code>
<!-- 
UNITDATAEDITED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|UnitDataEdited}}<b>(</b>'''int''' floatVarList, '''int''' memberCount, '''int''' memberIndex, '''bool''' isDebugFSM, {{Type5|SpecialistType}} specRender, '''bool''' isFromLua = nil<b>)</b></code>
<!-- 
DOFROMUIDIPLOEVENT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|DoFromUIDiploEvent}}<b>(</b>{{Type5|DiploUIEventType}} event, {{Type5|PlayerID}} aIPlayer, {{Type5|SpecialistType}} button, '''int''' againstPlayer, '''int''' arg3<b>)</b></code>
<!-- 
JOINMULTIPLAYERGAME
-->
|-
|align="right" width="200" |<code>'''unknown''', '''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Matchmaking}}.{{Func5|Matchmaking|JoinMultiplayerGame}}<b>(</b>{{Type5|SpecialistType}} server<b>)</b></code>
<!-- 
CANLOADCLOUDSAVE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Modding}}.{{Func5|Modding|CanLoadCloudSave}}<b>(</b>{{Type5|SpecialistType}} selected<b>)</b></code>
<!-- 
GETCLOUDSAVEREQUIREMENTS
-->
|-
|align="right" width="200" |<code>'''unknown''', '''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|Modding}}.{{Func5|Modding|GetCloudSaveRequirements}}<b>(</b>{{Type5|SpecialistType}} selected<b>)</b></code>
<!-- 
SENDDIPLOVOTE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendDiploVote}}<b>(</b>{{Type5|SpecialistType}} votePlayer<b>)</b></code>
<!-- 
CANPREPARE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanPrepare}}<b>(</b>{{Type5|SpecialistType}} specialist, '''bool''' continue<b>)</b></code>
<!-- 
GETDEALMYVALUE
-->
|-
|align="right" width="200" |<code>{{Type5|SpecialistType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetDealMyValue}}<b>(</b>{{Type5|Deal}} Deal<b>)</b></code>
<!-- 
GETRECENTINTRIGUEINFO
-->
|-
|align="right" width="200" |<code>{{Type5|SpecialistType}}, '''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetRecentIntrigueInfo}}<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>
<!-- 
GETSPECIALISTEXTRAYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetSpecialistExtraYield}}<b>(</b>{{Type5|SpecialistType}} index1, {{Type5|YieldType}} index2<b>)</b></code>
<!-- 
SPECIALISTYIELD
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SpecialistYield}}<b>(</b>{{Type5|SpecialistType}} specialist, {{Type5|YieldType}} yield<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|RadioButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|SpecialistType}} void1, '''int''' Control<b>)</b>) ModeClicked<b>)</b></code>
<!-- 
COPYLASTAUTOSAVETOSTEAMCLOUD
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Steam}}.{{Func5|Steam|CopyLastAutoSaveToSteamCloud}}<b>(</b>{{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
GETCLOUDSAVES
-->
|-
|align="right" width="200" |<code>table({{Type5|SpecialistType}} => {{Type5|FileHeader}})</code>
|style="padding-left:6px" |<code>{{Type5|Steam}}.{{Func5|Steam|GetCloudSaves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXCLOUDSAVES
-->
|-
|align="right" width="200" |<code>{{Type5|SpecialistType}}</code>
|style="padding-left:6px" |<code>{{Type5|Steam}}.{{Func5|Steam|GetMaxCloudSaves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SAVEGAMETOCLOUD
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Steam}}.{{Func5|Steam|SaveGameToCloud}}<b>(</b>{{Type5|SpecialistType}} slot<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TextButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|SpecialistType}} ePlayer<b>)</b>) OnCancelEditPlayerDetails<b>)</b></code>
<!-- 
GETREPLAYFILES
-->
|-
|align="right" width="200" |<code>table({{Type5|SpecialistType}} => '''unknown''')</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetReplayFiles}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LOADCURRENTDEAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|LoadCurrentDeal}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
LOADHISTORICDEAL
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|LoadHistoricDeal}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
SAVEFILELIST
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|SaveFileList}}<b>(</b>table({{Type5|SpecialistType}} => '''bool''') FileList, {{Type5|GameType}} GameType, '''bool''' ShowAutoSaves, '''bool''' arg3<b>)</b></code>
<!-- 
CANJOIN
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|CanJoin}}<b>(</b>{{Type5|Plot}} plot, {{Type5|SpecialistType}} specialist<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|SpecialistType]]
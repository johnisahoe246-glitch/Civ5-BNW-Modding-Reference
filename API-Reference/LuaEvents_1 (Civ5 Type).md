{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



= Usage =
This object provides a mechanism modders can use to define and subscribe their own events. Those events are then visible in all [[Context (Civ5 Type)|contexts]] and all mods.


To define a custom event, you just need to subscribe it or invoke it, the event will then be lazily created and no error will be thrown.<br/>
The following example defines a "VelociratproAttack" event and subscribes a "RunAway" handler to it.
<syntaxhighlight lang="lua" class="civ5-example">
function RunAway(name)
	print("Run "..name.."!")
end
LuaEvents.VelociraptorAttack.Add(RunAway)

-- Now fires the event. Prints "Run Forest!"
LuaEvents.VelociraptorAttack("Forest")
</syntaxhighlight>


=Events declared by the UI=
Events can be subscribed by using <code>LuaEvents.SomeEvent.Add(SomeFunction)</code>. Regular events can also be fired through a '''dot''' by using <code>LuaEvents.SomeEvent(&lt;args&gt;)</code>. This will invoke all subscribers with the provided arguments.<br/>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDITIONALINFORMATIONDROPDOWNGATHERENTRIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|AdditionalInformationDropdownGatherEntries}}<b>(</b>table('''int''' => '''table''') additionalEntries<b>)</b></code>
<!-- 
ADDITIONALINFORMATIONDROPDOWNSORTENTRIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|AdditionalInformationDropdownSortEntries}}<b>(</b>table('''int''' => '''table''') entries<b>)</b></code>
<!-- 
ADVISORBUTTONEVENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|AdvisorButtonEvent}}<b>(</b>{{Type5|MouseType}} button<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CHATSHOW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ChatShow}}<b>(</b>'''int''' chatOpen<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ENEMYPANELHIDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|EnemyPanelHide}}<b>(</b>'''bool''' isHide<b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MODBROWSERSETDELETEBUTTONSTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ModBrowserSetDeleteButtonState}}<b>(</b>..., '''bool''' arg1, '''string''' arg2 = nil<b>)</b></code>
<!-- 
MODBROWSERSETDOWNLOADBUTTONSTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ModBrowserSetDownloadButtonState}}<b>(</b>'''bool''' arg0, '''bool''' arg1<b>)</b></code>
<!-- 
MODBROWSERSETLIKEBUTTONSTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ModBrowserSetLikeButtonState}}<b>(</b>'''bool''' arg0, '''bool''' arg1<b>)</b></code>
<!-- 
MODBROWSERSETREPORTBUTTONSTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ModBrowserSetReportButtonState}}<b>(</b>'''bool''' arg0, '''bool''' arg1<b>)</b></code>
|}

==O==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ONMODBROWSERDELETEBUTTONCLICKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|OnModBrowserDeleteButtonClicked}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ONMODBROWSERDOWNLOADBUTTONCLICKED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|OnModBrowserDownloadButtonClicked}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ONMODSBROWSERNAVIGATEBACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|OnModsBrowserNavigateBack}}<b>(</b>'''table''' args<b>)</b></code>
<!-- 
ONRECOMMENDATIONCHECKCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|OnRecommendationCheckChanged}}<b>(</b>'''bool''' value<b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PASSWORDCHANGED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|PasswordChanged}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
PRODUCTIONPOPUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ProductionPopup}}<b>(</b>'''bool''' isHide<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
REPLAYVIEWER_LOADREPLAY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ReplayViewer_LoadReplay}}<b>(</b>'''unknown''' replayFile<b>)</b></code>
<!-- 
REQUESTREFRESHADDITIONALINFORMATIONDROPDOWNENTRIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|RequestRefreshAdditionalInformationDropdownEntries}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SCENARIOPLAYERSTATUSCHANGED
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ScenarioPlayerStatusChanged}}<b>(</b>table({{Type5|PlayerID}} => table('''string''' => '''table''')) tPlayerStatus, {{Type5|PlayerID}} turn, '''int''' year, {{Type5|PlayerID}} playerAboutToWin, '''int''' turnsControlHeld<b>)</b></code>
<!-- 
SCENARIOUNITTIERSCHANGED
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|ScenarioUnitTiersChanged}}<b>(</b>table('''string''' => {{Type5|PlayerID}}) tUnitTiers<b>)</b></code>
<!-- 
SETCIVNAMEEDITSLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|SetCivNameEditSlot}}<b>(</b>{{Type5|PlayerID}} slot<b>)</b></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TRYDISMISSTUTORIAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|TryDismissTutorial}}<b>(</b>'''string''' tutorialID<b>)</b></code>
<!-- 
TRYQUEUETUTORIAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|TryQueueTutorial}}<b>(</b>'''string''' tutorialID, '''bool''' highPriority<b>)</b></code>
|}


=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>LuaEvents.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADD
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|Add}}<!-- No arguments --></code>
<!-- 
CALL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|Call}}<!-- No arguments --></code>
<!-- 
COUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|Count}}<!-- No arguments --></code>
<!-- 
REMOVE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|Remove}}<!-- No arguments --></code>
<!-- 
REMOVEALL
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|LuaEvents|RemoveAll}}<!-- No arguments --></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|LuaEvents]]
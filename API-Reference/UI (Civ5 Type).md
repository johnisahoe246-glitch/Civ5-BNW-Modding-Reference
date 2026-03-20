{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>UI.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ACTIVATENOTIFICATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ActivateNotification}}<b>(</b>{{Type5|PlayerID}} blockingNotificationIndex<b>)</b></code>
<!-- 
ADDPOPUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|AddPopup}}<b>(</b>'''table''' popupInfo<b>)</b></code>
<!-- 
AREMEDIUMLEADERSALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|AreMediumLeadersAllowed}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANDOINTERFACEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|CanDoInterfaceMode}}<b>(</b>{{Type5|InterfaceMode}} interfaceMode<b>)</b></code>
<!-- 
CANENDTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|CanEndTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANPLACEUNITAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|CanPlaceUnitAt}}<b>(</b>'''unknown''' unit, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
CANSELECTIONLISTFOUND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|CanSelectionListFound}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANSELECTIONLISTWORK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|CanSelectionListWork}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGESTARTDIPLOREPEATCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ChangeStartDiploRepeatCount}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
CHECKFORCOMMANDLINEINVITATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|CheckForCommandLineInvitation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARPLACEUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ClearPlaceUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARSELECTEDCITIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ClearSelectedCities}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARSELECTIONLIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ClearSelectionList}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COMPAREFILETIME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|CompareFileTime}}<b>(</b>'''unknown''' arg0, '''unknown''' arg1, '''unknown''' arg2, '''unknown''' arg3<b>)</b></code>
<!-- 
COPYLASTAUTOSAVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|CopyLastAutoSave}}<b>(</b>'''string''' arg0<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DEBUGFLAG
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|DebugFlag}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DEBUGKEYHANDLER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DebugKeyHandler}}<b>(</b>{{Type5|KeyEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b></code>
<!-- 
DECTURNTIMERSEMAPHORE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|decTurnTimerSemaphore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DELETEREPLAYFILE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DeleteReplayFile}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
DELETESAVEDGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DeleteSavedGame}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
DODEMAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DoDemand}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOEQUALIZEDEALWITHHUMAN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DoEqualizeDealWithHuman}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOFINALIZEPLAYERDEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DoFinalizePlayerDeal}}<b>(</b>{{Type5|PlayerID}} them, {{Type5|PlayerID}} us, '''bool''' arg2<b>)</b></code>
<!-- 
DOPROPOSEDEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DoProposeDeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOSELECTCITYATPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DoSelectCityAtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
DOWHATDOESAIWANT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DoWhatDoesAIWant}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOWHATWILLAIGIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|DoWhatWillAIGive}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
EXITGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ExitGame}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCREDITS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetCredits}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCURRENTGAMESTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|GameStateType}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetCurrentGameState}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHALLOFFAMEDATA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''table''')</code>
|width="100%" |<code>{{FuncLabel5|UI|GetHallofFameData}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHEADSELECTEDCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|City}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetHeadSelectedCity}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHEADSELECTEDUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Unit}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetHeadSelectedUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINTERFACEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|InterfaceMode}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetInterfaceMode}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINTERFACEMODEDEBUGITEMID1
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetInterfaceModeDebugItemID1}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINTERFACEMODEDEBUGITEMID2
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|UnitType}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetInterfaceModeDebugItemID2}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINTERFACEMODEVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TaskType}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetInterfaceModeValue}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAPPLAYERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table({{Type5|UnitType}} => '''Civilizations.row''')</code>
|width="100%" |<code>{{FuncLabel5|UI|GetMapPlayers}}<b>(</b>'''string''' mapScriptPath<b>)</b></code>
<!-- 
GETMAPPREVIEW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|WorldBuilderMapData}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetMapPreview}}<b>(</b>'''string''' mapFilePath<b>)</b></code>
<!-- 
GETMOUSEOVERHEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetMouseOverHex}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCURRENTDEALS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetNumCurrentDeals}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNUMHISTORICDEALS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetNumHistoricDeals}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETPLACEUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetPlaceUnit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREPLAYFILEHEADER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FileHeader}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetReplayFileHeader}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
GETREPLAYFILES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table({{Type5|SpecialistType}} => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|UI|GetReplayFiles}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREPLAYINFO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ReplayInfo}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetReplayInfo}}<b>(</b>'''string''' file<b>)</b></code>
<!-- 
GETREPLAYMODIFICATIONTIME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetReplayModificationTime}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
GETREPLAYMODIFICATIONTIMERAW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetReplayModificationTimeRaw}}<b>(</b>'''unknown''' v<b>)</b></code>
<!-- 
GETSAVEDGAMEMODIFICATIONTIME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetSavedGameModificationTime}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
GETSAVEDGAMEMODIFICATIONTIMERAW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetSavedGameModificationTimeRaw}}<b>(</b>'''bool''' v<b>)</b></code>
<!-- 
GETSCRATCHDEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Deal}}</code>
|width="100%" |<code>{{FuncLabel5|UI|GetScratchDeal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETTEMPSTRING
-->
|-
{{FuncInfos5|yes  |maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetTempString}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVERSIONINFO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|UI|GetVersionInfo}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASMADEPROPOSAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|UI|HasMadeProposal}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
HASSHOWNLEGAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|HasShownLegal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HIGHLIGHTCANPLACEPLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|HighlightCanPlacePlots}}<b>(</b>{{Type5|Unit}} unit, {{Type5|Plot}} arg1<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
INCTURNTIMERSEMAPHORE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|incTurnTimerSemaphore}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
INTERRUPTTURNTIMER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|interruptTurnTimer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISAIREQUESTINGCONCESSIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|IsAIRequestingConcessions}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCAMERAMOVING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|IsCameraMoving}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCITYSCREENUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|IsCityScreenUp}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISCITYSCREENVIEWINGMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|IsCityScreenViewingMode}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISDX9
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|IsDX9}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISLOADEDGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|IsLoadedGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISMAPSCENARIO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|IsMapScenario}}<b>(</b>'''string''' mapScriptFileName<b>)</b></code>
|}

==L==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
LOADCURRENTDEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|LoadCurrentDeal}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
LOADHISTORICDEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|LoadHistoricDeal}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
LOADPROPOSEDDEAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|LoadProposedDeal}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them<b>)</b></code>
<!-- 
LOCATIONSELECT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|LocationSelect}}<b>(</b>{{Type5|Plot}} plot, '''int''' ctrl, '''int''' alt, '''bool''' shift<b>)</b></code>
<!-- 
LOOKAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|LookAt}}<b>(</b>{{Type5|Plot}} plot, '''int''' arg1 = nil<b>)</b></code>
<!-- 
LOOKATSELECTIONPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|LookAtSelectionPlot}}<b>(</b>'''int''' arg0<b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MOVESCENARIOPLAYERTOSLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|MoveScenarioPlayerToSlot}}<b>(</b>{{Type5|UnitType}} playerIndex, '''int''' arg1<b>)</b></code>
|}

==O==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ONHUMANDEMAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|OnHumanDemand}}<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>
<!-- 
ONHUMANOPENEDTRADESCREEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|OnHumanOpenedTradeScreen}}<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PROPOSEDDEALEXISTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|ProposedDealExists}}<b>(</b>{{Type5|PlayerID}} them, {{Type5|PlayerID}} us<b>)</b></code>
|}

==Q==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
QUICKSAVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|QuickSave}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
REBROADCASTNOTIFICATIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|RebroadcastNotifications}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REFRESHYIELDVISIBLEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|RefreshYieldVisibleMode}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REMOVENOTIFICATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|RemoveNotification}}<b>(</b>{{Type5|EndTurnBlockingType}} blockingNotificationIndex<b>)</b></code>
<!-- 
REQUESTLEAVELEADER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|RequestLeaveLeader}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REQUESTMINIMAPBROADCAST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|RequestMinimapBroadcast}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RESETSCENARIOPLAYERSLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ResetScenarioPlayerSlots}}<b>(</b>'''bool''' arg0 = nil<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SAVEFILELIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SaveFileList}}<b>(</b>table({{Type5|SpecialistType}} => '''bool''') FileList, {{Type5|GameType}} GameType, '''bool''' ShowAutoSaves, '''bool''' arg3<b>)</b></code>
<!-- 
SAVEGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SaveGame}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
SAVEMAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SaveMap}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
SELECTCITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SelectCity}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
SELECTUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SelectUnit}}<b>(</b>{{Type5|Unit}} v<b>)</b></code>
<!-- 
SENDPATHFINDERUPDATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SendPathfinderUpdate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETADVISORMESSAGEHASBEENSEEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetAdvisorMessageHasBeenSeen}}<b>(</b>'''unknown''' arg0, '''bool''' arg1<b>)</b></code>
<!-- 
SETCITYSCREENVIEWINGMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetCityScreenViewingMode}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETDIRTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetDirty}}<b>(</b>{{Type5|InterfaceDirtyBits}} arg0, '''bool''' arg1<b>)</b></code>
<!-- 
SETDONTSHOWPOPUPS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetDontShowPopups}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETGRIDVISIBLEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetGridVisibleMode}}<b>(</b>'''bool''' isChecked<b>)</b></code>
<!-- 
SETINTERFACEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetInterfaceMode}}<b>(</b>{{Type5|InterfaceMode}} interfaceModeSelection<b>)</b></code>
<!-- 
SETINTERFACEMODEVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetInterfaceModeValue}}<b>(</b>{{Type5|PlayerID}} minorCiv<b>)</b></code>
<!-- 
SETLEADERHEADROOTUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetLeaderHeadRootUp}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETOFFERTRADEREPEATCOUNT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetOfferTradeRepeatCount}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
SETPLACEUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetPlaceUnit}}<b>(</b>{{Type5|Unit}} unit<b>)</b></code>
<!-- 
SETREPEATACTIONPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetRepeatActionPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETRESOURCEVISIBLEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetResourceVisibleMode}}<b>(</b>'''bool''' isChecked<b>)</b></code>
<!-- 
SETYIELDVISIBLEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|SetYieldVisibleMode}}<b>(</b>'''bool''' isChecked<b>)</b></code>
<!-- 
SHIFTKEYDOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UI|ShiftKeyDown}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TOGGLEGRIDVISIBLEMODE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|ToggleGridVisibleMode}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UNLOCKACHIEVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|UnlockAchievement}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
UPDATECITYSCREEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UI|UpdateCityScreen}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==W==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
WAITINGFORREMOTEPLAYERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UI|WaitingForRemotePlayers}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|UI]]
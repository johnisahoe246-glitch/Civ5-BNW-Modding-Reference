{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>PreGame.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANREADYLOCALPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|CanReadyLocalPlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARDLCALLOWED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|ClearDLCAllowed}}<!-- No arguments --></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCIVILIZATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|CivilizationType}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilization}}<b>(</b>{{Type5|PlayerID}} i = nil<b>)</b></code>
<!-- 
GETCIVILIZATIONADJECTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilizationAdjective}}<b>(</b>'''int''' EditSlot<b>)</b></code>
<!-- 
GETCIVILIZATIONCOLOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilizationColor}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETCIVILIZATIONDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilizationDescription}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETCIVILIZATIONKEY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilizationKey}}<!-- No arguments --></code>
<!-- 
GETCIVILIZATIONPACKAGEID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilizationPackageID}}<!-- No arguments --></code>
<!-- 
GETCIVILIZATIONPACKAGETEXTKEY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilizationPackageTextKey}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETCIVILIZATIONSHORTDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetCivilizationShortDescription}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETERA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|EraType}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetEra}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFILEHEADER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FileHeader}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetFileHeader}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
GETGAMEOPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetGameOption}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
GETGAMESPEED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|GameSpeedType}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetGameSpeed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGAMETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|GameType}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetGameType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHANDICAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|HandicapType}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetHandicap}}<b>(</b>{{Type5|PlayerID}} player = nil<b>)</b></code>
<!-- 
GETLEADERKEY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetLeaderKey}}<!-- No arguments --></code>
<!-- 
GETLEADERNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetLeaderName}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETLEADERPACKAGEID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetLeaderPackageID}}<!-- No arguments --></code>
<!-- 
GETLEADERPACKAGETEXTKEY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetLeaderPackageTextKey}}<!-- No arguments --></code>
<!-- 
GETLEADERTYPE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetLeaderType}}<!-- No arguments --></code>
<!-- 
GETLOADFILENAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetLoadFileName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLOADWBSCENARIO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetLoadWBScenario}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAPOPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetMapOption}}<b>(</b>{{Type5|MapOptionID}} arg0<b>)</b></code>
<!-- 
GETMAPSCRIPT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetMapScript}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXTURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetMaxTurns}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMULTIPLAYERAIENABLED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetMultiplayerAIEnabled}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNICKNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetNickName}}<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>
<!-- 
GETNUMMINORCIVS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetNumMinorCivs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOVERRIDESCENARIOHANDICAP
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetOverrideScenarioHandicap}}<!-- No arguments --></code>
<!-- 
GETPASSWORD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetPassword}}<b>(</b>'''int''' EditSlot<b>)</b></code>
<!-- 
GETPERSISTSETTINGS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetPersistSettings}}<!-- No arguments --></code>
<!-- 
GETQUICKCOMBAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetQuickCombat}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETQUICKMOVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetQuickMovement}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSLOTCLAIM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|SlotClaim}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetSlotClaim}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETSLOTSTATUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|SlotStatus}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetSlotStatus}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TeamID}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetTeam}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETWORLDSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|HandicapType}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|GetWorldSize}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASPASSWORD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|HasPassword}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISCIVILIZATIONKEYAVAILABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsCivilizationKeyAvailable}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISDLCALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsDLCAllowed}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
ISEARTHMAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsEarthMap}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHOTSEATGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsHotSeatGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISINTERNETGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsInternetGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISLEADERKEYAVAILABLE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsLeaderKeyAvailable}}<!-- No arguments --></code>
<!-- 
ISMULTIPLAYERGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsMultiplayerGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISPRIVATEGAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsPrivateGame}}<!-- No arguments --></code>
<!-- 
ISRANDOMMAPSCRIPT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsRandomMapScript}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISRANDOMWORLDSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsRandomWorldSize}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISREADY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsReady}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISVICTORY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|IsVictory}}<b>(</b>'''string''' arg0<b>)</b></code>
|}

==L==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
LOADPREGAMESETTINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|LoadPreGameSettings}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
RANDOMIZEMAPSEED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|RandomizeMapSeed}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
READACTIVESLOTCOUNTFROMSAVEGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|ReadActiveSlotCountFromSaveGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RESET
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|Reset}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RESETGAMEOPTIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|ResetGameOptions}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RESETMAPOPTIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|ResetMapOptions}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RESETSLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|ResetSlots}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETCIVILIZATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetCivilization}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|CivilizationType}} civ = nil<b>)</b></code>
<!-- 
SETCIVILIZATIONADJECTIVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetCivilizationAdjective}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETCIVILIZATIONDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetCivilizationDescription}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETCIVILIZATIONKEY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetCivilizationKey}}<!-- No arguments --></code>
<!-- 
SETCIVILIZATIONPACKAGEID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetCivilizationPackageID}}<!-- No arguments --></code>
<!-- 
SETCIVILIZATIONSHORTDESCRIPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetCivilizationShortDescription}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETDLCALLOWED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetDLCAllowed}}<b>(</b>'''unknown''' arg0, '''bool''' check<b>)</b></code>
<!-- 
SETEARTHMAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetEarthMap}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETERA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetEra}}<b>(</b>{{Type5|EraType}} id<b>)</b></code>
<!-- 
SETGAMEOPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetGameOption}}<b>(</b>'''string''' arg0, '''bool''' check<b>)</b></code>
<!-- 
SETGAMESPEED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetGameSpeed}}<b>(</b>{{Type5|GameSpeedType}} id<b>)</b></code>
<!-- 
SETGAMETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetGameType}}<b>(</b>{{Type5|GameType}} gameType<b>)</b></code>
<!-- 
SETHANDICAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetHandicap}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|HandicapType}} id<b>)</b></code>
<!-- 
SETINTERNETGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetInternetGame}}<b>(</b>'''int''' isInternet<b>)</b></code>
<!-- 
SETLEADERKEY
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetLeaderKey}}<!-- No arguments --></code>
<!-- 
SETLEADERNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetLeaderName}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETLEADERPACKAGEID
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetLeaderPackageID}}<!-- No arguments --></code>
<!-- 
SETLEADERTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetLeaderType}}<b>(</b>'''int''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
SETLOADFILENAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetLoadFileName}}<b>(</b>'''string''' thisLoadFile, '''bool''' arg1 = nil<b>)</b></code>
<!-- 
SETLOADWBSCENARIO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetLoadWBScenario}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
SETMAPOPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetMapOption}}<b>(</b>'''unknown''' arg0, '''bool''' check<b>)</b></code>
<!-- 
SETMAPSCRIPT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetMapScript}}<b>(</b>'''string''' CurrentMap<b>)</b></code>
<!-- 
SETMAXTURNS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetMaxTurns}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
SETMULTIPLAYERAIENABLED
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetMultiplayerAIEnabled}}<!-- No arguments --></code>
<!-- 
SETMULTIPLAYERGAME
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetMultiplayerGame}}<!-- No arguments --></code>
<!-- 
SETNICKNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetNickName}}<b>(</b>{{Type5|PlayerID}} EditSlot, '''string''' arg1<b>)</b></code>
<!-- 
SETNUMMINORCIVS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetNumMinorCivs}}<b>(</b>'''int''' numMinorCivsWanted<b>)</b></code>
<!-- 
SETOVERRIDESCENARIOHANDICAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetOverrideScenarioHandicap}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETPASSWORD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetPassword}}<b>(</b>{{Type5|PlayerID}} player, '''string''' arg1, '''string''' arg2 = nil<b>)</b></code>
<!-- 
SETPERSISTSETTINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetPersistSettings}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETPLAYERCOLOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetPlayerColor}}<b>(</b>'''int''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
SETPRIVATEGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetPrivateGame}}<b>(</b>'''int''' checked<b>)</b></code>
<!-- 
SETQUICKCOMBAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetQuickCombat}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
SETQUICKMOVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetQuickMovement}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
SETRANDOMMAPSCRIPT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetRandomMapScript}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETRANDOMWORLDSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetRandomWorldSize}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETREADY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetReady}}<b>(</b>{{Type5|PlayerID}} arg0, '''bool''' checked = nil<b>)</b></code>
<!-- 
SETSLOTCLAIM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetSlotClaim}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|SlotClaim}} arg1<b>)</b></code>
<!-- 
SETSLOTSTATUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetSlotStatus}}<b>(</b>{{Type5|PlayerID}} i, {{Type5|SlotStatus}} arg1<b>)</b></code>
<!-- 
SETTEAM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetTeam}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|PlayerID}} playerChoice<b>)</b></code>
<!-- 
SETVICTORY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetVictory}}<b>(</b>{{Type5|VictoryType}} arg0, '''bool''' check<b>)</b></code>
<!-- 
SETWORLDSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PreGame|SetWorldSize}}<b>(</b>{{Type5|HandicapType}} id<b>)</b></code>
|}

==T==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TESTPASSWORD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|PreGame|TestPassword}}<b>(</b>{{Type5|PlayerID}} player, '''string''' arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|PreGame]]
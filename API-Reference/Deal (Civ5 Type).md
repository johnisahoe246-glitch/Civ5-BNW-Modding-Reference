{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Deal.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDALLOWEMBASSY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddAllowEmbassy}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
ADDCITYTRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddCityTrade}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|ResourceType}} city<b>)</b></code>
<!-- 
ADDDECLARATIONOFFRIENDSHIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddDeclarationOfFriendship}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
ADDDEFENSIVEPACT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddDefensivePact}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDGOLDPERTURNTRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddGoldPerTurnTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' goldPerTurn, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDGOLDTRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddGoldTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' amount<b>)</b></code>
<!-- 
ADDMAPTRADE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|AddMapTrade}}<!-- No arguments --></code>
<!-- 
ADDOPENBORDERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddOpenBorders}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDPEACETREATY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddPeaceTreaty}}<b>(</b>{{Type5|PlayerID}} us, '''int''' arg1<b>)</b></code>
<!-- 
ADDPERMAMENTALLIANCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|AddPermamentAlliance}}<!-- No arguments --></code>
<!-- 
ADDRESEARCHAGREEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddResearchAgreement}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDRESOURCETRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddResourceTrade}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resource, '''int''' amount, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDSURRENDER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|AddSurrender}}<!-- No arguments --></code>
<!-- 
ADDTHIRDPARTYEMBARGO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|AddThirdPartyEmbargo}}<!-- No arguments --></code>
<!-- 
ADDTHIRDPARTYPEACE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddThirdPartyPeace}}<b>(</b>{{Type5|PlayerID}} who, {{Type5|TeamID}} otherPlayer, '''int''' arg2<b>)</b></code>
<!-- 
ADDTHIRDPARTYWAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddThirdPartyWar}}<b>(</b>{{Type5|PlayerID}} who, {{Type5|TeamID}} otherPlayer<b>)</b></code>
<!-- 
ADDTRADEAGREEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|AddTradeAgreement}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
ADDTRUCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|AddTruce}}<!-- No arguments --></code>
<!-- 
ADDUNITTRADE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|AddUnitTrade}}<!-- No arguments --></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CHANGEGOLDPERTURNTRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|ChangeGoldPerTurnTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' goldPerTurn, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
CHANGEGOLDTRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|ChangeGoldTrade}}<b>(</b>{{Type5|PlayerID}} us, '''int''' gold<b>)</b></code>
<!-- 
CHANGERESOURCETRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|ChangeResourceTrade}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resource, '''int''' numResource, {{Type5|ResourceType}} dealDuration<b>)</b></code>
<!-- 
CHANGETHIRDPARTYEMBARGODURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|ChangeThirdPartyEmbargoDuration}}<!-- No arguments --></code>
<!-- 
CHANGETHIRDPARTYPEACEDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|ChangeThirdPartyPeaceDuration}}<!-- No arguments --></code>
<!-- 
CHANGETHIRDPARTYWARDURATION
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|ChangeThirdPartyWarDuration}}<!-- No arguments --></code>
<!-- 
CLEARITEMS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|ClearItems}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETDEMANDINGPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetDemandingPlayer}}<!-- No arguments --></code>
<!-- 
GETDURATION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetDuration}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETENDTURN
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetEndTurn}}<!-- No arguments --></code>
<!-- 
GETFROMPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetFromPlayer}}<!-- No arguments --></code>
<!-- 
GETGOLDAVAILABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetGoldAvailable}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|TradeableItemType}} itemToBeChanged<b>)</b></code>
<!-- 
GETNEXTITEM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TradeableItemType}}, '''unknown''', '''unknown''', {{Type5|ResourceType}}, '''int''', {{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetNextItem}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMITEMS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetNumItems}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetNumResource}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|ResourceType}} resType<b>)</b></code>
<!-- 
GETOTHERPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetOtherPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETREQUESTINGPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetRequestingPlayer}}<!-- No arguments --></code>
<!-- 
GETSTARTTURN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetStartTurn}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSURRENDERINGPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetSurrenderingPlayer}}<!-- No arguments --></code>
<!-- 
GETTOPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|GetToPlayer}}<!-- No arguments --></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISPOSSIBLETOTRADEITEM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Deal|IsPossibleToTradeItem}}<b>(</b>{{Type5|PlayerID}} us, {{Type5|PlayerID}} them, {{Type5|TradeableItemType}} tradeType, {{Type5|TeamID}} dealDuration, {{Type5|ResourceType}} dealDuration = nil<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
REMOVEBYTYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|RemoveByType}}<b>(</b>{{Type5|TradeableItemType}} arg0, {{Type5|PlayerID}} us<b>)</b></code>
<!-- 
REMOVECITYTRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|RemoveCityTrade}}<b>(</b>{{Type5|SpecialistType}} player, '''int''' cityID<b>)</b></code>
<!-- 
REMOVERESOURCETRADE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|RemoveResourceTrade}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
REMOVETHIRDPARTYEMBARGO
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|RemoveThirdPartyEmbargo}}<!-- No arguments --></code>
<!-- 
REMOVETHIRDPARTYPEACE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|RemoveThirdPartyPeace}}<b>(</b>{{Type5|PlayerID}} firstParty, {{Type5|TeamID}} otherPlayer<b>)</b></code>
<!-- 
REMOVETHIRDPARTYWAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|RemoveThirdPartyWar}}<b>(</b>{{Type5|PlayerID}} firstParty, {{Type5|TeamID}} otherPlayer<b>)</b></code>
<!-- 
REMOVEUNITTRADE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|RemoveUnitTrade}}<!-- No arguments --></code>
<!-- 
RESETITERATOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|ResetIterator}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETDEMANDINGPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|SetDemandingPlayer}}<!-- No arguments --></code>
<!-- 
SETFROMPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|SetFromPlayer}}<b>(</b>{{Type5|PlayerID}} us<b>)</b></code>
<!-- 
SETREQUESTINGPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|SetRequestingPlayer}}<!-- No arguments --></code>
<!-- 
SETSURRENDERINGPLAYER
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Deal|SetSurrenderingPlayer}}<!-- No arguments --></code>
<!-- 
SETTOPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Deal|SetToPlayer}}<b>(</b>{{Type5|PlayerID}} them<b>)</b></code>
|}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETDEALMYVALUE
-->
|-
|align="right" width="200" |<code>{{Type5|SpecialistType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetDealMyValue}}<b>(</b>{{Type5|Deal}} Deal<b>)</b></code>
<!-- 
GETSCRATCHDEAL
-->
|-
|align="right" width="200" |<code>{{Type5|Deal}}</code>
|style="padding-left:6px" |<code>{{Type5|UI}}.{{Func5|UI|GetScratchDeal}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Deal]]
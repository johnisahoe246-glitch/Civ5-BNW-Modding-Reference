{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This object is defined in the following Lua source file: ''Amazon_XP.lua''.
:To import it, use: <code>include("Amazon_XP")</code>}}


=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>AssignStartingPlots.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CREATE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|Create}}<b>(</b><!-- No arguments --><b>)</b></code>
|}


=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of AssignStartingPlots.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
==_==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
__CUSTOMINIT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|__CustomInit}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
__INIT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|__Init}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
__INITLUXURYWEIGHTS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|__InitLuxuryWeights}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDEXTRABONUSESTOHILLSREGIONS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AddExtraBonusesToHillsRegions}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDMODERNMINORSTRATEGICSTOCITYSTATES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AddModernMinorStrategicsToCityStates}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDSTRATEGICBALANCERESOURCES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AddStrategicBalanceResources}}<b>(</b>'''int''' region_number<b>)</b></code>
<!-- 
APPLYHEXADJUSTMENT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ApplyHexAdjustment}}<b>(</b>'''int''' x, '''int''' y, table('''int''' => '''int''') plot_adjustments<b>)</b></code>
<!-- 
ASSIGNCITYSTATESTOREGIONSORTOUNINHABITED
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AssignCityStatesToRegionsOrToUninhabited}}<b>(</b>'''unknown''' args<b>)</b></code>
<!-- 
ASSIGNLUXURYROLES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AssignLuxuryRoles}}<!-- No arguments --></code>
<!-- 
ASSIGNLUXURYTOREGION
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AssignLuxuryToRegion}}<b>(</b>{{Type5|PlayerID}} region_number<b>)</b></code>
<!-- 
ATTEMPTTOPLACEBONUSRESOURCEATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AttemptToPlaceBonusResourceAtPlot}}<b>(</b>'''int''' x, '''int''' y, '''bool''' allowOasis<b>)</b></code>
<!-- 
ATTEMPTTOPLACEHILLSATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AttemptToPlaceHillsAtPlot}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
ATTEMPTTOPLACENATURALWONDER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AttemptToPlaceNaturalWonder}}<b>(</b>'''int''' wonder_number, '''int''' row_number<b>)</b></code>
<!-- 
ATTEMPTTOPLACESMALLSTRATEGICATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AttemptToPlaceSmallStrategicAtPlot}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
ATTEMPTTOPLACESTONEATGRASSPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|AttemptToPlaceStoneAtGrassPlot}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
|}

==B==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
BALANCEANDASSIGN
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|BalanceAndAssign}}<!-- No arguments --></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANBECRATER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeCrater}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBEFUJI
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeFuji}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBEGEYSER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeGeyser}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBEGIBRALTAR
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeGibraltar}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBEKRAKATOA
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeKrakatoa}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBEMESA
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeMesa}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBEMTSINAI
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeMtSinai}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBERAREMYSTICAL
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeRareMystical}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBEREEF
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeReef}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CANBETHISNATURALWONDERTYPE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanBeThisNaturalWonderType}}<b>(</b>'''int''' x, '''int''' y, '''int''' wn, '''int''' rn<b>)</b></code>
<!-- 
CANPLACECITYSTATEAT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CanPlaceCityStateAt}}<b>(</b>'''int''' x, '''int''' y, {{Type5|AreaID}} area_ID, '''int''' force_it, '''int''' ignore_collisions<b>)</b></code>
<!-- 
CHOOSELOCATIONS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ChooseLocations}}<b>(</b>'''int''' args<b>)</b></code>
<!-- 
CHOPINTOTHREEREGIONS
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ChopIntoThreeRegions}}<b>(</b>'''unknown''' fertility_table, '''table''' rectangle_data_table, '''bool''' taller, '''unknown''' chopPercent = nil<b>)</b></code>
<!-- 
CHOPINTOTWOREGIONS
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ChopIntoTwoRegions}}<b>(</b>'''unknown''' fertility_table, '''table''' rectangle_data_table, '''bool''' taller, '''float''' chopPercent<b>)</b></code>
<!-- 
CUSTOMOVERRIDE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''int''', '''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|CustomOverride}}<b>(</b>{{Type5|ResourceType}} resource_<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DETERMINEREGIONTYPES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|DetermineRegionTypes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DIVIDEBRITAIN
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|DivideBritain}}<b>(</b>'''int''' numDivisions, '''unknown''' fertility_table, '''int''' rectangle_data_table<b>)</b></code>
<!-- 
DIVIDEINTOREGIONS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|DivideIntoRegions}}<b>(</b>'''int''' numDivisions, '''unknown''' fertility_table, '''table''' rectangle_data_table<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
EVALUATECANDIDATEPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|EvaluateCandidatePlot}}<b>(</b>'''int''' plotIndex, '''int''' region_type<b>)</b></code>
<!-- 
EXAMINECANDIDATEPLOTFORNATURALWONDERSELIGIBILITY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ExamineCandidatePlotForNaturalWondersEligibility}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
EXAMINEPLOTFORNATURALWONDERSELIGIBILITY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ExaminePlotForNaturalWondersEligibility}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
|}

==F==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
FINDCOASTALSTART
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool''', '''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|FindCoastalStart}}<b>(</b>'''int''' region_number<b>)</b></code>
<!-- 
FINDFALLBACKFORUNMATCHEDREGIONPRIORITY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|FindFallbackForUnmatchedRegionPriority}}<b>(</b>'''int''' regionType, table('''int''' => {{Type5|PlayerID}}) regions_still_available<b>)</b></code>
<!-- 
FINDSTART
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool''', '''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|FindStart}}<b>(</b>'''int''' region_number<b>)</b></code>
<!-- 
FINDSTARTWITHOUTREGARDTOAREAID
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool''', '''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|FindStartWithoutRegardToAreaID}}<b>(</b>'''int''' region_number, '''bool''' mustBeCoast<b>)</b></code>
<!-- 
FIXSUGARJUNGLES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|FixSugarJungles}}<!-- No arguments --></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GENERATEGLOBALRESOURCEPLOTLISTS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GenerateGlobalResourcePlotLists}}<!-- No arguments --></code>
<!-- 
GENERATELOCALVERSIONSOFDATAFROMXML
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GenerateLocalVersionsOfDataFromXML}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATELUXURYPLOTLISTSATCITYSITE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GenerateLuxuryPlotListsAtCitySite}}<b>(</b>'''int''' x, '''int''' y, '''int''' radius, '''bool''' removeFeatureIce<b>)</b></code>
<!-- 
GENERATELUXURYPLOTLISTSINREGION
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GenerateLuxuryPlotListsInRegion}}<b>(</b>{{Type5|PlayerID}} region_number<b>)</b></code>
<!-- 
GENERATENATURALWONDERSCANDIDATEPLOTLISTS
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''int''')</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GenerateNaturalWondersCandidatePlotLists}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATEREGIONS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GenerateRegions}}<b>(</b>'''int''' args<b>)</b></code>
<!-- 
GETCITYSTATELUXURIESTARGETNUMBER
-->
|-
{{FuncInfos5|maybe|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetCityStateLuxuriesTargetNumber}}<!-- No arguments --></code>
<!-- 
GETDISABLEDLUXURIESTARGETNUMBER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetDisabledLuxuriesTargetNumber}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINDICESFORLUXURYTYPE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int''', '''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetIndicesForLuxuryType}}<b>(</b>{{Type5|ResourceType}} resource_<b>)</b></code>
<!-- 
GETLISTOFALLOWABLELUXURIESATCITYSITE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetListOfAllowableLuxuriesAtCitySite}}<b>(</b>'''int''' x, '''int''' y, '''int''' radius<b>)</b></code>
<!-- 
GETLUXURIESSPLITCAP
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetLuxuriesSplitCap}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAJORSTRATEGICRESOURCEQUANTITYVALUES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetMajorStrategicResourceQuantityValues}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETREGIONLUXURYTARGETNUMBERS
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetRegionLuxuryTargetNumbers}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSMALLSTRATEGICRESOURCEQUANTITYVALUES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}, {{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetSmallStrategicResourceQuantityValues}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWORLDLUXURYTARGETNUMBERS
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|GetWorldLuxuryTargetNumbers}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
IDENTIFYREGIONSOFTHISTYPE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|IdentifyRegionsOfThisType}}<b>(</b>'''int''' region_type<b>)</b></code>
<!-- 
ITERATETHROUGHCANDIDATEPLOTLIST
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|IterateThroughCandidatePlotList}}<b>(</b>table('''int''' => '''int''') plot_list, '''int''' region_type<b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MEASURESINGLEPLOT
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|MeasureSinglePlot}}<b>(</b>'''int''' x, '''int''' y, '''int''' region_type<b>)</b></code>
<!-- 
MEASURESTARTPLACEMENTFERTILITYINRECTANGLE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|MeasureStartPlacementFertilityInRectangle}}<b>(</b>'''int''' westX, '''int''' southY, '''int''' width, '''int''' height<b>)</b></code>
<!-- 
MEASURESTARTPLACEMENTFERTILITYOFLANDMASS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', {{Type5|AreaID}}, {{Type5|AreaID}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|MeasureStartPlacementFertilityOfLandmass}}<b>(</b>{{Type5|AreaID}} areaID, {{Type5|AreaID}} westX, '''int''' eastX, {{Type5|AreaID}} southY, '''int''' northY, '''bool''' wrapsX, '''bool''' wrapsY<b>)</b></code>
<!-- 
MEASURESTARTPLACEMENTFERTILITYOFPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|MeasureStartPlacementFertilityOfPlot}}<b>(</b>'''int''' x, '''int''' y, '''bool''' checkForCoastalLand<b>)</b></code>
<!-- 
MEASURETERRAININREGIONS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|MeasureTerrainInRegions}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==N==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
NORMALIZECITYSTATE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|NormalizeCityState}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
NORMALIZECITYSTATELOCATIONS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|NormalizeCityStateLocations}}<!-- No arguments --></code>
<!-- 
NORMALIZESTARTLOCATION
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|NormalizeStartLocation}}<b>(</b>'''int''' region_number<b>)</b></code>
<!-- 
NORMALIZETEAMLOCATIONS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|NormalizeTeamLocations}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==O==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
OBTAINNEXTSECTIONINREGION
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''int'''), table('''int''' => '''int'''), '''unknown''', '''unknown''', '''unknown''', '''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ObtainNextSectionInRegion}}<b>(</b>'''int''' incoming_west_x, '''int''' incoming_south_y, '''int''' incoming_width, '''int''' incoming_height, {{Type5|AreaID}} areaID, '''int''' force_it, '''int''' ignore_collisions<b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PLACECITYSTATE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int''', '''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceCityState}}<b>(</b>table('''int''' => '''int''') coastal_plot_list, table('''int''' => '''int''') inland_plot_list, '''bool''' check_proximity, '''bool''' check_collision<b>)</b></code>
<!-- 
PLACECITYSTATEINREGION
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceCityStateInRegion}}<b>(</b>'''int''' city_state_number, {{Type5|PlayerID}} region_number<b>)</b></code>
<!-- 
PLACECITYSTATES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceCityStates}}<!-- No arguments --></code>
<!-- 
PLACEFISH
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceFish}}<b>(</b>'''int''' frequency, table('''int''' => {{Type5|PlayerID}}) plot_list<b>)</b></code>
<!-- 
PLACEIMPACTANDRIPPLES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceImpactAndRipples}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
PLACELUXURIES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceLuxuries}}<!-- No arguments --></code>
<!-- 
PLACEMARBLE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceMarble}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PLACENATURALWONDERS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceNaturalWonders}}<!-- No arguments --></code>
<!-- 
PLACEOILINTHESEA
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceOilInTheSea}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PLACERESOURCEIMPACT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceResourceImpact}}<b>(</b>'''int''' x, '''int''' y, '''int''' impact_table_number, '''int''' radius<b>)</b></code>
<!-- 
PLACERESOURCESANDCITYSTATES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceResourcesAndCityStates}}<!-- No arguments --></code>
<!-- 
PLACESEXYBONUSATCIVSTARTS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceSexyBonusAtCivStarts}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PLACESMALLQUANTITIESOFSTRATEGICS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceSmallQuantitiesOfStrategics}}<b>(</b>'''int''' frequency, table('''int''' => '''int''') plot_list<b>)</b></code>
<!-- 
PLACESPECIFICNUMBEROFRESOURCES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceSpecificNumberOfResources}}<b>(</b>{{Type5|ResourceType}} resource_, {{Type5|ResourceType}} quantity, '''int''' amount, '''float''' ratio, '''int''' impact_table_number, '''int''' min_radius, '''int''' max_radius, table('''int''' => {{Type5|PlayerID}}) plot_list<b>)</b></code>
<!-- 
PLACESTRATEGICANDBONUSRESOURCES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PlaceStrategicAndBonusResources}}<!-- No arguments --></code>
<!-- 
PRINTFINALRESOURCETOTALSTOLOG
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|PrintFinalResourceTotalsToLog}}<!-- No arguments --></code>
<!-- 
PROCESSRESOURCELIST
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|ProcessResourceList}}<b>(</b>'''int''' frequency, '''int''' impact_table_number, table('''int''' => '''int''') plot_list, table('''int''' => table('''int''' => {{Type5|ResourceType}})) resources_to_place<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
REMOVEDEADROWS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''int'''), '''int''', '''int''', '''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|RemoveDeadRows}}<b>(</b>table('''int''' => '''int''') fertility_table, '''int''' westX, '''int''' southY, '''int''' width, '''int''' height<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SORTREGIONSBYTYPE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AssignStartingPlots|SortRegionsByType}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|AssignStartingPlots]]
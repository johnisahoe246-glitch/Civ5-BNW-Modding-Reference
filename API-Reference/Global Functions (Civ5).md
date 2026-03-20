{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



<div class="toclimit-2"> __TOC__</div>
=Built-in functions=
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDRESOURCETYPE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AddResourceType}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGEBUILDINGSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|ChangeBuildingSize}}<b>(</b>'''float''' arg0<b>)</b></code>
<!-- 
FOW_SETALL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FOW_SetAll}}<b>(</b>{{Type5|FogOfWarModeType}} fogOfWarType<b>)</b></code>
<!-- 
GETENDTURNTIMERLENGTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|getEndTurnTimerLength}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOVERLAYLEGEND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|OverlayInfo}})</code>
|width="100%" |<code>{{FuncLabel5|GetOverlayLegend}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTRATEGICVIEWICONSETTINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table({{Type5|InfoCornerID}} => '''string''')</code>
|width="100%" |<code>{{FuncLabel5|GetStrategicViewIconSettings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSTRATEGICVIEWOVERLAYS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table({{Type5|InfoCornerID}} => '''string''')</code>
|width="100%" |<code>{{FuncLabel5|GetStrategicViewOverlays}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVOLUMEKNOBIDFROMNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ActionType}}</code>
|width="100%" |<code>{{FuncLabel5|GetVolumeKnobIDFromName}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
GETVOLUMEKNOBVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|GetVolumeKnobValue}}<b>(</b>{{Type5|ActionType}} musicVolumeKnob<b>)</b></code>
<!-- 
GRIDTOWORLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|GridToWorld}}<b>(</b>{{Type5|ResourceType}} gridX, '''int''' gridY<b>)</b></code>
<!-- 
HEXTOWORLD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector3}}</code>
|width="100%" |<code>{{FuncLabel5|HexToWorld}}<b>(</b>{{Type5|Vector2}} hexPos<b>)</b></code>
<!-- 
ICE_RELOAD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Ice_Reload}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
INSTRATEGICVIEW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|InStrategicView}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LOOKUPCONTROL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Context}}</code>
|width="100%" |<code>{{FuncLabel5|LookUpControl}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
MOUSEOVERSTRATEGICVIEWRESOURCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|MouseOverStrategicViewResource}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
PROCESSSTRATEGICVIEWMOUSECLICK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|ProcessStrategicViewMouseClick}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
RELOADTEXTURES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|ReloadTextures}}<b>(</b>'''int''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
RESETACHIEVEMENTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|ResetAchievements}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SAVEAUDIOOPTIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|SaveAudioOptions}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETSELECTEDCIV
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|SetSelectedCiv}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETSTRATEGICVIEWICONSETTING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|SetStrategicViewIconSetting}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
SETSTRATEGICVIEWOVERLAY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|SetStrategicViewOverlay}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
SETVOLUMEKNOBVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|SetVolumeKnobValue}}<b>(</b>{{Type5|ActionType}} musicVolumeKnob, '''int''' cachedMusicVolumeKnob<b>)</b></code>
<!-- 
STRATEGICVIEWSHOWFEATURES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|StrategicViewShowFeatures}}<b>(</b>'''bool''' isChecked<b>)</b></code>
<!-- 
STRATEGICVIEWSHOWFOGOFWAR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|StrategicViewShowFogOfWar}}<b>(</b>'''bool''' isChecked<b>)</b></code>
<!-- 
TOGGLEPAUSEGAMEPLAY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TogglePauseGameplay}}<b>(</b>'''bool''' pauseGameplay<b>)</b></code>
<!-- 
TOGGLESTRATEGICVIEW
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|ToggleStrategicView}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
TOGRIDFROMHEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}, {{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|ToGridFromHex}}<b>(</b>'''float''' i, '''float''' j<b>)</b></code>
<!-- 
TOHEXFROMGRID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector2}}</code>
|width="100%" |<code>{{FuncLabel5|ToHexFromGrid}}<b>(</b>{{Type5|Vector2}} gridPos<b>)</b></code>
<!-- 
UNITMOVING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UnitMoving}}<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit<b>)</b></code>
<!-- 
WATER_SETAMPLITUDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Water_SetAmplitude}}<b>(</b>'''int''' waterAmplitude<b>)</b></code>
<!-- 
WATER_SETAUTORELOAD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Water_SetAutoReload}}<b>(</b>'''bool''' waterReload<b>)</b></code>
<!-- 
WATER_SETFLOWPARAMETERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Water_SetFlowParameters}}<b>(</b>'''int''' waterFlowStrength, '''int''' waterNoiseStrength, '''int''' waterNoiseScale<b>)</b></code>
<!-- 
WATER_SETGRADIENTSCALE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Water_SetGradientScale}}<b>(</b>'''int''' waterGradientScale<b>)</b></code>
<!-- 
WATER_SETSCALE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Water_SetScale}}<b>(</b>'''int''' waterScale<b>)</b></code>
<!-- 
WATER_SETSPEC
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Water_SetSpec}}<b>(</b>'''int''' waterSunSpec, '''int''' waterSkySpec<b>)</b></code>
<!-- 
WATER_SETSPEED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Water_SetSpeed}}<b>(</b>'''int''' waterScrollSpeed<b>)</b></code>
<!-- 
WAVES_RELOAD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Waves_Reload}}<b>(</b><!-- No arguments --><b>)</b></code>
|}


=FLuaVector.lua=
Those functions are declared in '''FLuaVector.lua'''. Use: <code>include("FLuaVector")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
COLOR
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector4}}</code>
|width="100%" |<code>{{FuncLabel5|Color}}<b>(</b>'''float''' r, '''float''' g, '''float''' b, '''float''' a<b>)</b></code>
<!-- 
VECADD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|VecAdd}}<b>(</b>'''unknown''' v1, '''unknown''' v2<b>)</b></code>
<!-- 
VECSUBTRACT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|VecSubtract}}<b>(</b>'''unknown''' v1, '''unknown''' v2<b>)</b></code>
<!-- 
VECTOR2
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector2}}</code>
|width="100%" |<code>{{FuncLabel5|Vector2}}<b>(</b>'''float''' i, '''float''' j<b>)</b></code>
<!-- 
VECTOR3
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector3}}</code>
|width="100%" |<code>{{FuncLabel5|Vector3}}<b>(</b>'''float''' i, '''float''' j, '''float''' k<b>)</b></code>
<!-- 
VECTOR4
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector4}}</code>
|width="100%" |<code>{{FuncLabel5|Vector4}}<b>(</b>'''float''' i, '''float''' j = nil, '''float''' k = nil, '''float''' l = nil<b>)</b></code>
|}


=GameCalendarUtilities.lua=
Those functions are declared in '''GameCalendarUtilities.lua'''. Use: <code>include("GameCalendarUtilities")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETDATESTRING
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetDateString}}<b>(</b>'''int''' gameTurn, '''unknown''' calendarType, '''unknown''' gameSpeedType, '''int''' startYear<b>)</b></code>
<!-- 
GETDEFAULTYEARSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetDefaultYearString}}<b>(</b>'''int''' year<b>)</b></code>
<!-- 
GETSHORTDATESTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetShortDateString}}<b>(</b>'''int''' gameTurn, '''unknown''' calendarType, '''unknown''' gameSpeedType, '''int''' startYear<b>)</b></code>
|}


=IconSupport.lua=
Those functions are declared in '''IconSupport.lua'''. Use: <code>include("IconSupport")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CIVICONHOOKUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|CivIconHookup}}<b>(</b>{{Type5|PlayerID}} player, '''int''' iconSize, {{Type5|Image}} iconControl, {{Type5|Image}} teamColorControl, '''int''' shadowIconControl, '''int''' alwaysUseComposite, '''int''' shadowed<b>)</b></code>
<!-- 
ICONHOOKUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|IconHookup}}<b>(</b>'''int''' offset, '''float''' iconSize, '''string''' atlas, {{Type5|Image}} imageControl, '''unknown''' debugPrint = nil<b>)</b></code>
<!-- 
ICONLOOKUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector2}}, '''string'''</code>
|width="100%" |<code>{{FuncLabel5|IconLookup}}<b>(</b>'''int''' offset, '''int''' iconSize, '''string''' atlas<b>)</b></code>
<!-- 
POPULATEICONATLASES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PopulateIconAtlases}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SIMPLECIVICONHOOKUP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|SimpleCivIconHookup}}<b>(</b>{{Type5|PlayerID}} player, '''int''' iconSize, {{Type5|Image}} iconControl<b>)</b></code>
|}


=InfoTooltipInclude.lua=
Those functions are declared in '''InfoTooltipInclude.lua'''. Use: <code>include("InfoTooltipInclude")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCITYSTATESTATUS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetCityStateStatus}}<b>(</b>{{Type5|Player}} player, {{Type5|PlayerID}} forPlayer, '''int''' war<b>)</b></code>
<!-- 
GETCULTURETOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetCultureTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETFAITHTOOLTIP
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetFaithTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETFOODTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetFoodTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETGOLDTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetGoldTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETHELPTEXTFORBUILDING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetHelpTextForBuilding}}<b>(</b>{{Type5|BuildingType}} building, '''bool''' excludeName, '''bool''' excludeHeader, '''bool''' noMaintenance<b>)</b></code>
<!-- 
GETHELPTEXTFORIMPROVEMENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetHelpTextForImprovement}}<b>(</b>{{Type5|ImprovementType}} improvement, '''bool''' excludeName, '''bool''' excludeHeader, '''bool''' noMaintenance<b>)</b></code>
<!-- 
GETHELPTEXTFORPROJECT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetHelpTextForProject}}<b>(</b>{{Type5|ProjectType}} project, '''bool''' includeRequirementsInfo<b>)</b></code>
<!-- 
GETHELPTEXTFORUNIT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetHelpTextForUnit}}<b>(</b>{{Type5|UnitType}} unit, '''bool''' includeRequirementsInfo<b>)</b></code>
<!-- 
GETMOODINFO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetMoodInfo}}<b>(</b>{{Type5|PlayerID}} otherPlayer<b>)</b></code>
<!-- 
GETPRODUCTIONTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetProductionTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETRELIGIONTOOLTIP
-->
|-
{{FuncInfos5|no   |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetReligionTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETSCIENCETOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetScienceTooltip}}<b>(</b>{{Type5|City}} city<b>)</b></code>
<!-- 
GETYIELDTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetYieldTooltip}}<b>(</b>{{Type5|City}} city, {{Type5|YieldType}} yieldType, '''int''' base, '''int''' total, '''string''' iconString, '''string''' modifiersString<b>)</b></code>
<!-- 
GETYIELDTOOLTIPHELPER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetYieldTooltipHelper}}<b>(</b>{{Type5|City}} city, {{Type5|YieldType}} yieldType, '''string''' icon<b>)</b></code>
|}


=MapGenerator.lua=
Those functions are declared in '''MapGenerator.lua'''. Use: <code>include("MapGenerator")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADDFEATURES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AddFeatures}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDGOODIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AddGoodies}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDLAKES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|AddLakes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDRIVERS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|AddRivers}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANPLACEGOODYAT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|CanPlaceGoodyAt}}<b>(</b>{{Type5|ImprovementType}} improvement, {{Type5|Plot}} plot<b>)</b></code>
<!-- 
DETERMINECONTINENTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|DetermineContinents}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DORIVER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|DoRiver}}<b>(</b>{{Type5|Plot}} startPlot, {{Type5|FlowDirectionType}} thisFlowDirection = nil, {{Type5|FlowDirectionType}} originalFlowDirection = nil, '''int''' riverID = nil<b>)</b></code>
<!-- 
GENERATECOASTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GenerateCoasts}}<b>(</b>'''int''' args = nil<b>)</b></code>
<!-- 
GENERATEMAP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GenerateMap}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATEPLOTTYPES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GeneratePlotTypes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATETERRAIN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GenerateTerrain}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCOREMAPOPTIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''...'''</code>
|width="100%" |<code>{{FuncLabel5|GetCoreMapOptions}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOPPOSITEFLOWDIRECTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|FlowDirectionType}}</code>
|width="100%" |<code>{{FuncLabel5|GetOppositeFlowDirection}}<b>(</b>{{Type5|FlowDirectionType}} dir<b>)</b></code>
<!-- 
GETRIVERVALUEATPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|GetRiverValueAtPlot}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
PLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator()</code>
|width="100%" |<code>{{FuncLabel5|Plots}}<b>(</b>('''void''' func<b>(</b>table('''int''' => '''int''') t<b>)</b>) sort = nil<b>)</b></code>
<!-- 
SETPLOTTYPES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|SetPlotTypes}}<b>(</b>table('''int''' => {{Type5|PlotType}}) plotTypes<b>)</b></code>
<!-- 
SETTERRAINTYPES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|SetTerrainTypes}}<b>(</b>table('''int''' => {{Type5|TerrainType}}) terrainTypes<b>)</b></code>
<!-- 
FUNC
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|func}}<b>(</b>table('''int''' => '''int''') t<b>)</b></code>
<!-- 
STARTPLOTSYSTEM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|StartPlotSystem}}<b>(</b><!-- No arguments --><b>)</b></code>
|}


=MapmakerUtilities.lua=
Those functions are declared in '''MapmakerUtilities.lua'''. Use: <code>include("MapmakerUtilities")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ADJACENTTOSALTWATER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|AdjacentToSaltWater}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
CIVNEEDSCOASTALSTART
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|CivNeedsCoastalStart}}<b>(</b>'''string''' civType<b>)</b></code>
<!-- 
CIVNEEDSRIVERSTART
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|CivNeedsRiverStart}}<b>(</b>'''string''' civType<b>)</b></code>
<!-- 
GENERATECOASTALLANDDATATABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''bool''')</code>
|width="100%" |<code>{{FuncLabel5|GenerateCoastalLandDataTable}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GENERATENEXTTOCOASTALLANDDATATABLES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''bool'''), table('''int''' => '''int''')</code>
|width="100%" |<code>{{FuncLabel5|GenerateNextToCoastalLandDataTables}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMSTARTREGIONAVOIDFORCIV
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|GetNumStartRegionAvoidForCiv}}<b>(</b>'''string''' civType<b>)</b></code>
<!-- 
GETNUMSTARTREGIONPRIORITYFORCIV
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|GetNumStartRegionPriorityForCiv}}<b>(</b>'''string''' civType<b>)</b></code>
<!-- 
GETPLAYERANDTEAMINFO
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int''', table('''int''' => {{Type5|PlayerID}}), '''bool''', table('''int''' => '''int'''), '''table'''</code>
|width="100%" |<code>{{FuncLabel5|GetPlayerAndTeamInfo}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSHUFFLEDCOPYOFTABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|PlayerID}})</code>
|width="100%" |<code>{{FuncLabel5|GetShuffledCopyOfTable}}<b>(</b>table('''int''' => '''int''') incoming_table<b>)</b></code>
<!-- 
GETSTARTREGIONAVOIDLISTFORCIV_GETIDS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''int''')</code>
|width="100%" |<code>{{FuncLabel5|GetStartRegionAvoidListForCiv_GetIDs}}<b>(</b>'''string''' civType<b>)</b></code>
<!-- 
GETSTARTREGIONAVOIDLISTFORCIV_GETTYPES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GetStartRegionAvoidListForCiv_GetTypes}}<b>(</b>'''unknown''' civType<b>)</b></code>
<!-- 
GETSTARTREGIONPRIORITYLISTFORCIV_GETIDS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''int''')</code>
|width="100%" |<code>{{FuncLabel5|GetStartRegionPriorityListForCiv_GetIDs}}<b>(</b>'''string''' civType<b>)</b></code>
<!-- 
GETSTARTREGIONPRIORITYLISTFORCIV_GETTYPES
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|GetStartRegionPriorityListForCiv_GetTypes}}<b>(</b>'''unknown''' civType<b>)</b></code>
<!-- 
IDENTIFYTABLEINDEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool''', '''int''', table('''int''' => '''int''')</code>
|width="100%" |<code>{{FuncLabel5|IdentifyTableIndex}}<b>(</b>table('''int''' => {{Type5|PlayerID}}) incoming_table, {{Type5|PlayerID}} value<b>)</b></code>
<!-- 
OBTAINLANDMASSBOUNDARIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''int''')</code>
|width="100%" |<code>{{FuncLabel5|ObtainLandmassBoundaries}}<b>(</b>{{Type5|AreaID}} areaID<b>)</b></code>
<!-- 
PRINTCONTENTSOFTABLE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|PrintContentsOfTable}}<b>(</b>table('''int''' => '''int''') incoming_table<b>)</b></code>
<!-- 
TESTMEMBERSHIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TestMembership}}<b>(</b>table('''int''' => {{Type5|PlayerID}}) table, {{Type5|PlayerID}} value<b>)</b></code>
|}


=PlotMouseoverInclude.lua=
Those functions are declared in '''PlotMouseoverInclude.lua'''. Use: <code>include("PlotMouseoverInclude")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCIVSTATEQUESTSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetCivStateQuestString}}<b>(</b>{{Type5|Plot}} plot, '''bool''' shortVersion<b>)</b></code>
<!-- 
GETIMPROVEMENTSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetImprovementString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETNATURESTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetNatureString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETOWNERSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetOwnerString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETRESOURCESTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetResourceString}}<b>(</b>{{Type5|Plot}} plot, '''bool''' longForm<b>)</b></code>
<!-- 
GETUNITSSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetUnitsString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
GETYIELDSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|GetYieldString}}<b>(</b>{{Type5|Plot}} plot<b>)</b></code>
<!-- 
ISFEATURESPECIAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|IsFeatureSpecial}}<b>(</b>{{Type5|FeatureType}} feature<b>)</b></code>
|}


=SupportFunctions.lua=
Those functions are declared in '''SupportFunctions.lua'''. Use: <code>include("SupportFunctions")</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
TRUNCATESTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TruncateString}}<b>(</b>{{Type5|Label}} control, '''int''' resultSize, '''string''' longStr, '''string''' trailingText = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 API]]
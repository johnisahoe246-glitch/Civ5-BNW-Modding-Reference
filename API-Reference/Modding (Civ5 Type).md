{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Modding.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ACTIVATEALLOWEDDLC
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|ActivateAllowedDLC}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ACTIVATEDLC
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|ActivateDLC}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ACTIVATEENABLEDMODS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|ActivateEnabledMods}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ACTIVATEMODSANDDLCFORREPLAY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|ActivateModsAndDLCForReplay}}<b>(</b>'''unknown''' replayFile<b>)</b></code>
<!-- 
ACTIVATESPECIFICMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|ActivateSpecificMod}}<b>(</b>'''string''' tutorialModId, '''unknown''' tutorialModVersion<b>)</b></code>
<!-- 
ALLENABLEDMODSCONTAINPROPERTYVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|AllEnabledModsContainPropertyValue}}<b>(</b>'''string''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
ANYACTIVATEDMODSCONTAINPROPERTYVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|AnyActivatedModsContainPropertyValue}}<b>(</b>'''string''' arg0, '''string''' arg1<b>)</b></code>
<!-- 
ANYENABLEDMODSCONTAINPROPERTYVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|AnyEnabledModsContainPropertyValue}}<b>(</b>'''string''' arg0, '''int''' arg1<b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CANDELETEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|CanDeleteMod}}<b>(</b>'''unknown''' modId, '''int''' modVersion<b>)</b></code>
<!-- 
CANENABLEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => '''int''')</code>
|width="100%" |<code>{{FuncLabel5|Modding|CanEnableMod}}<b>(</b>table('''int''' => '''table''') modsToTestCanEnable<b>)</b></code>
<!-- 
CANLOADCLOUDSAVE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|CanLoadCloudSave}}<b>(</b>{{Type5|SpecialistType}} selected<b>)</b></code>
<!-- 
CANLOADREPLAY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|CanLoadReplay}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
CANLOADSAVEDGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|CanLoadSavedGame}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
CANUNSUBSCRIBEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|CanUnsubscribeMod}}<b>(</b>'''unknown''' modId, '''int''' modVersion<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DEACTIVATEMODS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|DeactivateMods}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DELETEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|DeleteMod}}<b>(</b>'''unknown''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
DELETEUSERDATA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|DeleteUserData}}<b>(</b>'''unknown''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
DISABLEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|DisableMod}}<b>(</b>{{Type5|Button}} modID, {{Type5|Button}} version<b>)</b></code>
|}

==E==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ENABLEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|EnableMod}}<b>(</b>{{Type5|Button}} modID, {{Type5|Button}} version<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETACTIVATEDMODENTRYPOINTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetActivatedModEntryPoints}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
GETACTIVATEDMODS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetActivatedMods}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETACTIVATEDMODVERSION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetActivatedModVersion}}<b>(</b>'''string''' myModId<b>)</b></code>
<!-- 
GETCLOUDSAVEREQUIREMENTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetCloudSaveRequirements}}<b>(</b>{{Type5|SpecialistType}} selected<b>)</b></code>
<!-- 
GETDLCASSOCIATIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|ModDependency}})</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetDlcAssociations}}<b>(</b>'''string''' modId, '''int''' modVersion<b>)</b></code>
<!-- 
GETDLCNAMEDESCRIPTIONKEYS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetDlcNameDescriptionKeys}}<b>(</b>'''int''' packageId<b>)</b></code>
<!-- 
GETDOWNLOADPROGRESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetDownloadProgress}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
GETENABLEDMODSBYACTIVATIONORDER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetEnabledModsByActivationOrder}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEVALUATEDFILEPATH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetEvaluatedFilePath}}<b>(</b>'''string''' myModId, '''unknown''' myModVersion, '''string''' customImage<b>)</b></code>
<!-- 
GETGAMEVERSIONASSOCIATIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|ModDependency}})</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetGameVersionAssociations}}<b>(</b>'''string''' modId, '''int''' modVersion<b>)</b></code>
<!-- 
GETINSTALLEDFIRAXISSCENARIOS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator({{Type5|ScenarioInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetInstalledFiraxisScenarios}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINSTALLEDMODDETAILS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetInstalledModDetails}}<b>(</b>'''unknown''' modId, '''int''' modVersion<b>)</b></code>
<!-- 
GETINSTALLPROGRESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetInstallProgress}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLATESTINSTALLEDMODVERSION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetLatestInstalledModVersion}}<b>(</b>'''string''' tutorialModId<b>)</b></code>
<!-- 
GETMAPFILES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|MapFileInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetMapFiles}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMODASSOCIATIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|ModDependency}})</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetModAssociations}}<b>(</b>'''string''' modId, '''int''' modVersion<b>)</b></code>
<!-- 
GETMODBROWSERDOWNLOADINGLISTINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|ModInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetModBrowserDownloadingListings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMODBROWSERINSTALLEDLISTINGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''string''' => {{Type5|ModInfo}})</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetModBrowserInstalledListings}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMODPROPERTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetModProperty}}<b>(</b>'''unknown''' arg0, '''unknown''' arg1, '''string''' arg2<b>)</b></code>
<!-- 
GETMODSBROWSERINSTALLEDLISTINGSSTATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetModsBrowserInstalledListingsState}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMODSREQUIREDTODISABLEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetModsRequiredToDisableMod}}<b>(</b>{{Type5|Button}} modID, {{Type5|Button}} version<b>)</b></code>
<!-- 
GETREPLAYREQUIREMENTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetReplayRequirements}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
GETSAVEDGAMEREQUIREMENTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetSavedGameRequirements}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
GETSYSTEMPROPERTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|GetSystemProperty}}<b>(</b>'''string''' arg0<b>)</b></code>
|}

==H==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
HASPENDINGINSTALLS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|HasPendingInstalls}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASUSERDATA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|HasUserData}}<b>(</b>'''unknown''' arg0, '''int''' arg1<b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
INSTALLMODS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|InstallMods}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==O==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
OPENSAVEDATA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Slider}}</code>
|width="100%" |<code>{{FuncLabel5|Modding|OpenSaveData}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
OPENUSERDATA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Slider}}</code>
|width="100%" |<code>{{FuncLabel5|Modding|OpenUserData}}<b>(</b>'''string''' TutorialID, '''unknown''' latestTutorialVersion<b>)</b></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PERFORMACTIONS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|PerformActions}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
PUBLISHEDFILEIDSMATCH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Modding|PublishedFileIdsMatch}}<b>(</b>'''unknown''' arg0, '''unknown''' arg1<b>)</b></code>
|}

==S==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
SETSYSTEMPROPERTY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|SetSystemProperty}}<b>(</b>'''string''' arg0, '''string''' arg1<b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UNSUBSCRIBEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|UnsubscribeMod}}<b>(</b>'''unknown''' arg0, '''int''' arg1<b>)</b></code>
<!-- 
UPDATEMOD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|UpdateMod}}<b>(</b>{{Type5|Button}} arg0, {{Type5|Button}} arg1<b>)</b></code>
<!-- 
UPDATEMODDINGSYSTEM
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Modding|UpdateModdingSystem}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Modding]]
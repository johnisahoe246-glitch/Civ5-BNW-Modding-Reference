{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Steam.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ACTIVATEGAMEOVERLAY
-->
|-
{{FuncInfos5|maybe|maybe|yes|Activates game overlay to specific page}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Steam|ActivateGameOverlay}}<b>(</b>'''string''' page<b>)</b></code>
<!-- 
ACTIVATEGAMEOVERLAYTOSTORE
-->
|-
{{FuncInfos5|yes  |yes  |yes|Opens the built-in web browser of the overlay and navigates to a store page on Steam}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Steam|ActivateGameOverlayToStore}}<b>(</b>'''int''' storeID = nil<b>)</b></code>
<!-- 
ACTIVATEGAMEOVERLAYTOWEBPAGE
-->
|-
{{FuncInfos5|yes  |yes  |yes|Opens the built-in web browser of the overlay and navigates to the specified URL}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Steam|ActivateGameOverlayToWebPage}}<b>(</b>'''string''' url<b>)</b></code>
<!-- 
ACTIVATEINVITEOVERLAY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Steam|ActivateInviteOverlay}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
COPYLASTAUTOSAVETOSTEAMCLOUD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Steam|CopyLastAutoSaveToSteamCloud}}<b>(</b>{{Type5|SpecialistType}} i<b>)</b></code>
<!-- 
GETCLOUDSAVEFILENAME
-->
|-
{{FuncInfos5|yes  |yes  |yes|Obtains the fully qualified filename of a Cloud Save slot}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Steam|GetCloudSaveFileName}}<b>(</b>'''int''' slot<b>)</b></code>
<!-- 
GETCLOUDSAVES
-->
|-
{{FuncInfos5|yes  |yes  |yes|Obtains information about all Steam Cloud saved games}}
|align="right"  |<code>table({{Type5|SpecialistType}} => {{Type5|FileHeader}})</code>
|width="100%" |<code>{{FuncLabel5|Steam|GetCloudSaves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMAXCLOUDSAVES
-->
|-
{{FuncInfos5|yes  |yes  |yes|Returns the Max number of save slots allowed on the Cloud}}
|align="right"  |<code>{{Type5|SpecialistType}}</code>
|width="100%" |<code>{{FuncLabel5|Steam|GetMaxCloudSaves}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMYSTEAMID
-->
|-
{{FuncInfos5|maybe|maybe|yes|Returns information about the current user's Steam ID}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Steam|GetMySteamID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERSTEAMID
-->
|-
{{FuncInfos5|maybe|maybe|yes|Returns the Steam ID information for a specific Player}}
|align="right"  |<code>table('''unknown''' => '''unknown''')</code>
|width="100%" |<code>{{FuncLabel5|Steam|GetPlayerSteamID}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
ISOVERLAYENABLED
-->
|-
{{FuncInfos5|maybe|maybe|yes|Determines if the Steam overlay is currently being displayed}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Steam|IsOverlayEnabled}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SAVEGAMETOCLOUD
-->
|-
{{FuncInfos5|yes  |yes  |yes|Saves the current game to a cloud save slot.}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Steam|SaveGameToCloud}}<b>(</b>{{Type5|SpecialistType}} slot<b>)</b></code>
<!-- 
SETOVERLAYNOTIFICATIONPOSITION
-->
|-
{{FuncInfos5|yes  |yes  |yes|Adjusts where the overlay notification is displayed for the user}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Steam|SetOverlayNotificationPosition}}<b>(</b>'''string''' position = nil<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Steam]]
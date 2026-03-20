{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Matchmaking.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCURRENTGAMENAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|GetCurrentGameName}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFRIENDLIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|GetFriendList}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETHOSTID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|GetHostID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETLOCALID
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|PlayerID}}</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|GetLocalID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETMULTIPLAYERGAMELIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table('''int''' => {{Type5|MultiplayerGame}})</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|GetMultiplayerGameList}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPLAYERLIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>table({{Type5|PlayerID}} => '''table''')</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|GetPlayerList}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HOSTHOTSEATGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|HostHotSeatGame}}<b>(</b>'''string''' gameName, '''int''' arg1<b>)</b></code>
<!-- 
HOSTINTERNETGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|HostInternetGame}}<b>(</b>'''string''' gameName, '''int''' arg1<b>)</b></code>
<!-- 
HOSTLANGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|HostLANGame}}<b>(</b>'''string''' gameName, '''int''' arg1<b>)</b></code>
<!-- 
ISHOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|IsHost}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISLAUNCHINGGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|IsLaunchingGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
JOINMULTIPLAYERGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|JoinMultiplayerGame}}<b>(</b>{{Type5|SpecialistType}} server<b>)</b></code>
<!-- 
KICKPLAYER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|KickPlayer}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
LAUNCHMULTIPLAYERGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|LaunchMultiplayerGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LEAVEMULTIPLAYERGAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|LeaveMultiplayerGame}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REFRESHINTERNETGAMELIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|RefreshInternetGameList}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REFRESHLANGAMELIST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Matchmaking|RefreshLANGameList}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Matchmaking]]
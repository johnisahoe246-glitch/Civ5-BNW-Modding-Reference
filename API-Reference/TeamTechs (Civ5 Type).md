{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of TeamTechs.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CHANGERESEARCHPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|ChangeResearchProgress}}<b>(</b>{{Type5|TechType}} index, '''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESSPERCENT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|ChangeResearchProgressPercent}}<b>(</b>{{Type5|TechType}} index, '''int''' percent, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESSTIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|ChangeResearchProgressTimes100}}<b>(</b>{{Type5|TechType}} index, '''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETLASTTECHACQUIRED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|TechType}}</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|GetLastTechAcquired}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
GETNUMTECHSKNOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|GetNumTechsKnown}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
GETRESEARCHCOST
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|GetResearchCost}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
GETRESEARCHLEFT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|GetResearchLeft}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
GETRESEARCHPROGRESS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|GetResearchProgress}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
GETRESEARCHPROGRESSTIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|GetResearchProgressTimes100}}<!-- No arguments --></code>
<!-- 
GETTECHCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|GetTechCount}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
HASRESEARCHEDALLTECHS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|HasResearchedAllTechs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASTECH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|HasTech}}<b>(</b>'''int''' index<b>)</b></code>
<!-- 
INCREMENTTECHCOUNT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|IncrementTechCount}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
ISNOTRADETECH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|IsNoTradeTech}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
SETHASTECH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|SetHasTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETNOTRADETECH
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|SetNoTradeTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETRESEARCHPROGRESS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|SetResearchProgress}}<b>(</b>{{Type5|TechType}} index, '''int''' newValue, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
SETRESEARCHPROGRESSTIMES100
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|TeamTechs|SetResearchProgressTimes100}}<!-- No arguments --></code>
|}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETTEAMTECHS
-->
|-
|align="right" width="200" |<code>{{Type5|TeamTechs}}</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetTeamTechs}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|TeamTechs]]
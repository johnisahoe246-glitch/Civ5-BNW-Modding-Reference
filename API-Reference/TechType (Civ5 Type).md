{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>TechType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>TechType</code> corresponds to the ''ID'' column of the {{Table5|Technologies|CIV5Technologies}} XML table.
}}


= XML: the Technologies table =
Here are the ''ID'' and ''Type'' columns found in this table.
<code>
{|
|-
!align="left" |ID
!
!align="left" |Type
|-
|align="right"|0
|
|TECH_AGRICULTURE
|-
|align="right"|1
|
|TECH_POTTERY
|-
|align="right"|2
|
|TECH_ANIMAL_HUSBANDRY
|-
|align="right"|3
|
|TECH_ARCHERY
|-
|align="right"|4
|
|TECH_MINING
|-
|align="right"|5
|
|TECH_SAILING
|-
|align="right"|6
|
|TECH_CALENDAR
|-
|align="right"|7
|
|TECH_WRITING
|-
|align="right"|8
|
|TECH_TRAPPING
|-
|align="right"|9
|
|TECH_THE_WHEEL
|-
|align="right"|10
|
|TECH_MASONRY
|-
|align="right"|11
|
|TECH_BRONZE_WORKING
|-
|align="right"|12
|
|TECH_OPTICS
|-
|align="right"|13
|
|TECH_PHILOSOPHY
|-
|align="right"|14
|
|TECH_HORSEBACK_RIDING
|-
|align="right"|15
|
|TECH_MATHEMATICS
|-
|align="right"|16
|
|TECH_CONSTRUCTION
|-
|align="right"|17
|
|TECH_IRON_WORKING
|-
|align="right"|17
|
|TECH_DRAMA
|-
|align="right"|18
|
|TECH_THEOLOGY
|-
|align="right"|19
|
|TECH_CIVIL_SERVICE
|-
|align="right"|20
|
|TECH_CURRENCY
|-
|align="right"|21
|
|TECH_ENGINEERING
|-
|align="right"|22
|
|TECH_METAL_CASTING
|-
|align="right"|23
|
|TECH_COMPASS
|-
|align="right"|23
|
|TECH_GUILDS
|-
|align="right"|24
|
|TECH_EDUCATION
|-
|align="right"|25
|
|TECH_CHIVALRY
|-
|align="right"|26
|
|TECH_MACHINERY
|-
|align="right"|27
|
|TECH_PHYSICS
|-
|align="right"|28
|
|TECH_STEEL
|-
|align="right"|29
|
|TECH_ASTRONOMY
|-
|align="right"|30
|
|TECH_ACOUSTICS
|-
|align="right"|31
|
|TECH_BANKING
|-
|align="right"|32
|
|TECH_PRINTING_PRESS
|-
|align="right"|33
|
|TECH_GUNPOWDER
|-
|align="right"|34
|
|TECH_NAVIGATION
|-
|align="right"|35
|
|TECH_ECONOMICS
|-
|align="right"|36
|
|TECH_CHEMISTRY
|-
|align="right"|37
|
|TECH_METALLURGY
|-
|align="right"|37
|
|TECH_ARCHITECTURE
|-
|align="right"|38
|
|TECH_ARCHAEOLOGY
|-
|align="right"|39
|
|TECH_SCIENTIFIC_THEORY
|-
|align="right"|40
|
|TECH_MILITARY_SCIENCE
|-
|align="right"|41
|
|TECH_FERTILIZER
|-
|align="right"|42
|
|TECH_RIFLING
|-
|align="right"|43
|
|TECH_BIOLOGY
|-
|align="right"|43
|
|TECH_INDUSTRIALIZATION
|-
|align="right"|44
|
|TECH_STEAM_POWER
|-
|align="right"|45
|
|TECH_ELECTRICITY
|-
|align="right"|46
|
|TECH_REPLACEABLE_PARTS
|-
|align="right"|47
|
|TECH_RAILROAD
|-
|align="right"|48
|
|TECH_DYNAMITE
|-
|align="right"|49
|
|TECH_REFRIGERATION
|-
|align="right"|50
|
|TECH_TELEGRAPH
|-
|align="right"|51
|
|TECH_RADIO
|-
|align="right"|52
|
|TECH_FLIGHT
|-
|align="right"|53
|
|TECH_COMBUSTION
|-
|align="right"|54
|
|TECH_PLASTIC
|-
|align="right"|55
|
|TECH_PENICILIN
|-
|align="right"|56
|
|TECH_ELECTRONICS
|-
|align="right"|57
|
|TECH_MASS_MEDIA
|-
|align="right"|58
|
|TECH_RADAR
|-
|align="right"|58
|
|TECH_BALLISTICS
|-
|align="right"|59
|
|TECH_ATOMIC_THEORY
|-
|align="right"|60
|
|TECH_ECOLOGY
|-
|align="right"|61
|
|TECH_COMPUTERS
|-
|align="right"|62
|
|TECH_ROCKETRY
|-
|align="right"|63
|
|TECH_LASERS
|-
|align="right"|63
|
|TECH_COMBINED_ARMS
|-
|align="right"|64
|
|TECH_NUCLEAR_FISSION
|-
|align="right"|65
|
|TECH_GLOBALIZATION
|-
|align="right"|66
|
|TECH_ROBOTICS
|-
|align="right"|67
|
|TECH_SATELLITES
|-
|align="right"|68
|
|TECH_STEALTH
|-
|align="right"|68
|
|TECH_TELECOM
|-
|align="right"|69
|
|TECH_ADVANCED_BALLISTICS
|-
|align="right"|69
|
|TECH_MOBILE_TACTICS
|-
|align="right"|70
|
|TECH_PARTICLE_PHYSICS
|-
|align="right"|71
|
|TECH_NUCLEAR_FUSION
|-
|align="right"|72
|
|TECH_NANOTECHNOLOGY
|-
|align="right"|73
|
|TECH_FUTURE_TECH
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
NOTIFICATIONADDED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Events}}.{{Func5|Events|NotificationAdded}}<b>(</b>{{Type5|CityAIFocusType}} notification, {{Type5|NotificationType}} notificationType, '''string''' toolTip, '''string''' summary, '''int''' gameValue, {{Type5|TechType}} extraGameData<b>)</b></code>
<!-- 
COUNTKNOWNTECHNUMTEAMS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CountKnownTechNumTeams}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
ISTECHRECOMMENDED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsTechRecommended}}<b>(</b>{{Type5|TechType}} arg0, {{Type5|AdvisorType}} advisorLoop<b>)</b></code>
<!-- 
TEAMSETHASTECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|TeamSetHasTech}}<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''bool''' adopted<b>)</b></code>
<!-- 
TEAMTECHRESEARCHED
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|TeamTechResearched}}<b>(</b>{{Type5|TeamID}} team, {{Type5|TechType}} tech, '''int''' change<b>)</b></code>
<!-- 
SETVOID1
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Grid}}:{{Func5|UIElement|SetVoid1}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
SETVOIDS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Grid}}:{{Func5|UIElement|SetVoids}}<b>(</b>{{Type5|TechType}} void1, {{Type5|ResourceType}} void2<b>)</b></code>
<!-- 
CALCULATERESEARCHMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CalculateResearchModifier}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
CANEVERRESEARCH
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanEverResearch}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
CANRESEARCH
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanResearch}}<b>(</b>{{Type5|TechType}} tech, '''bool''' trade = false<b>)</b></code>
<!-- 
CANRESEARCHFORFREE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanResearchForFree}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
FINDPATHLENGTH
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|FindPathLength}}<b>(</b>{{Type5|TechType}} tech, '''bool''' cost<b>)</b></code>
<!-- 
GETADVANCEDSTARTTECHCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetAdvancedStartTechCost}}<b>(</b>{{Type5|TechType}} tech, '''bool''' add<b>)</b></code>
<!-- 
GETCURRENTRESEARCH
-->
|-
|align="right" width="200" |<code>{{Type5|TechType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetCurrentResearch}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETQUEUEPOSITION
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetQueuePosition}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
GETRESEARCHCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetResearchCost}}<b>(</b>{{Type5|TechType}} currentTech<b>)</b></code>
<!-- 
GETRESEARCHPROGRESS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetResearchProgress}}<b>(</b>{{Type5|TechType}} currentTech<b>)</b></code>
<!-- 
GETRESEARCHTURNSLEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetResearchTurnsLeft}}<b>(</b>{{Type5|TechType}} tech, '''bool''' overflow<b>)</b></code>
<!-- 
POPRESEARCH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|PopResearch}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
SETRESEARCHINGTECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetResearchingTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
ISHASTECH
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsHasTech}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
SETHASTECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|SetHasTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue, {{Type5|PlayerID}} player, '''bool''' first, '''bool''' announce<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|ChangeResearchProgress}}<b>(</b>{{Type5|TechType}} index, '''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESSPERCENT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|ChangeResearchProgressPercent}}<b>(</b>{{Type5|TechType}} index, '''int''' percent, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
CHANGERESEARCHPROGRESSTIMES100
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|ChangeResearchProgressTimes100}}<b>(</b>{{Type5|TechType}} index, '''int''' change, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETLASTTECHACQUIRED
-->
|-
|align="right" width="200" |<code>{{Type5|TechType}}</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|GetLastTechAcquired}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
GETNUMTECHSKNOWN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|GetNumTechsKnown}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
GETRESEARCHCOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|GetResearchCost}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
GETRESEARCHLEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|GetResearchLeft}}<b>(</b>{{Type5|TechType}} tech<b>)</b></code>
<!-- 
GETRESEARCHPROGRESS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|GetResearchProgress}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
GETTECHCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|GetTechCount}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
INCREMENTTECHCOUNT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|IncrementTechCount}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
ISNOTRADETECH
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|IsNoTradeTech}}<b>(</b>{{Type5|TechType}} index<b>)</b></code>
<!-- 
SETHASTECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|SetHasTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETNOTRADETECH
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|SetNoTradeTech}}<b>(</b>{{Type5|TechType}} index, '''bool''' newValue<b>)</b></code>
<!-- 
SETRESEARCHPROGRESS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|TeamTechs}}:{{Func5|TeamTechs|SetResearchProgress}}<b>(</b>{{Type5|TechType}} index, '''int''' newValue, {{Type5|PlayerID}} player<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|TechType]]
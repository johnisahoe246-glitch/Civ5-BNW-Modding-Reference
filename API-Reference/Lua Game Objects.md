Up: [[Lua and UI Reference]]


This page contains list of known objects available. Each object has it's own page with function list and documentation.

== Static Methods ==
Objects that have single instance.

* [[Lua Game Objects/DB|DB]] -- ''Generic database routines''
* [[Lua Game Objects/Events|Events]] -- ''Contains various events which are routed through the engine, principally those with UI relevance''
* [[Lua Game Objects/Game|Game]] -- ''Methods related to the currently active CvGame instance''
* [[Lua Game Objects/GameEvents|GameEvents]] -- ''Similar to [[Lua Game Objects/Events|Events]], but related to the game rules engine, rather than the UI''
* [[Lua Game Objects/GameInfo|GameInfo]] -- ''All game database is exposed over this object''
* [[Lua Game Objects/Locale|Locale]] -- ''Methods related to Localization''
* [[Lua Game Objects/LuaEvents|LuaEvents]] -- ''Dynamically created events which are sent to and from arbitrary Lua states''
* [[Lua Game Objects/Map|Map]] -- ''Methods related to the currently active CvMap instance''
* [[Lua Game Objects/Modding|Modding]] -- ''Modding and mod package management''
* [[Lua Game Objects/Network|Network]] -- ''TCP/IP and HTTP methods''
* [[Lua Game Objects/Path|Path]] -- ''Utilities for parsing standard paths''
* [[Lua Game Objects/PreGame|PreGame]] -- ''Used to setup a game''
* [[Lua Game Objects/Steam|Steam]] -- ''Steam overlay''
* [[Lua Game Objects/UI|UI]] -- ''User interface''

== Lua "Classes", or Scoped Methods ==
Classes can have many instances. They are usually returned as function results.

* [[Lua Game Objects/Area]]
* [[Lua Game Objects/City]]
* [[Lua Game Objects/Plot]]
* [[Lua Game Objects/Player]]
* [[Lua Game Objects/Team]]
* [[Lua Game Objects/TeamTech]]
* [[Lua Game Objects/Deal]]
* [[Lua Game Objects/Unit]]

== Lua Enums ==

* [[Lua Game Objects/ActionSubTypes]]
* [[Lua Game Objects/ActivityTypes]]
* [[Lua Game Objects/AICityStrategies]]
* [[Lua Game Objects/ButtonPopupTypes]]
* [[Lua Game Objects/ButtonStates]]
* [[Lua Game Objects/CityUpdateTypes]]
* [[Lua Game Objects/CommandTypes]]
* [[Lua Game Objects/DiploUIStateTypes]]
* [[Lua Game Objects/DirectionTypes]]
* [[Lua Game Objects/DomainTypes]]
* [[Lua Game Objects/EndTurnBlockingTypes]]
* [[Lua Game Objects/FeatureTypes]]
* [[Lua Game Objects/FlowDirectionTypes]]
* [[Lua Game Objects/FogOfWarModeTypes]]
* [[Lua Game Objects/FromUIDiploEventTypes]]
* [[Lua Game Objects/GameDefines]] -- ''Similar to GameInfo.Defines but indexed by GameDefines.Name.''
* [[Lua Game Objects/GameMessageTypes]]
* [[Lua Game Objects/InterfaceDirtyBits]]
* [[Lua Game Objects/InterfaceModeTypes]]
* [[Lua Game Objects/KeyEvents]]
* [[Lua Game Objects/Keys]]
* [[Lua Game Objects/LeaderheadAnimationTypes]]
* [[Lua Game Objects/MajorCivApproachTypes]]
* [[Lua Game Objects/MinorCivPersonalityTypes]]
* [[Lua Game Objects/MinorCivQuestTypes]]
* [[Lua Game Objects/MinorCivTraitTypes]]
* [[Lua Game Objects/MissionTypes]]
* [[Lua Game Objects/Mouse]]
* [[Lua Game Objects/MouseEvents]]
* [[Lua Game Objects/NotificationTypes]]
* [[Lua Game Objects/OrderTypes]]
* [[Lua Game Objects/PlotTypes]]
* [[Lua Game Objects/PolicyBranchTypes]]
* [[Lua Game Objects/ResourceUsageTypes]]
* [[Lua Game Objects/TaskTypes]]
* [[Lua Game Objects/TerrainTypes]]
* [[Lua Game Objects/TradeableItems]]
* [[Lua Game Objects/YieldDisplayTypes]]
* [[Lua Game Objects/YieldTypes]]

== How to get function names for other game objects ==

These lists are available in ModBuddy/Help/Civ5LuaAPI.html.

Alternatively, object metatable can be obtained by calling ''getmetatable'' on non-nil object pointer. Then it is possible to iterate over all values stored in __index variable.

'''Example:'''
<pre>
	local plot = Map.GetPlot(0, 0)
	print("Attributes:")
	for k, v in pairs(getmetatable(plot).__index) do print(k) end
	print("End attributes.");
</pre>
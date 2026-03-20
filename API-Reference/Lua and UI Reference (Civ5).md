{{Civ5 API Beta Banner}}

= Lua =
* [[Specificities of the Lua implementation in Civ5]]
* [[Lua introduction for confirmed developers]]
* [http://sourceforge.net/apps/mediawiki/civ4bug/index.php?title=Python_to_Lua Lua introduction for Python developers]
* [http://www.lua.org/manual/5.1/ Lua reference]
* [http://www.lua.org/pil/index.html Lua manual]


= Articles and tutorials =
See also [[Civ5 Modding Tutorials|Modding Tutorials]].
{|cellspacing="0" cellpadding="0"
|-
|valign="top" width="200"|
* [[Civ5 API FAQ]]
* [[Civ5 API Reference FAQ]]
* [[Lua Libraries for Civ5]]
|valign="top" width="200"|
* [[Map and terrain (Civ5)|Map and terrain]]
* [[Persisting data (Civ5)|Persisting data]]
|valign="top"|
* [http://forums.civfanatics.com/showthread.php?p=11575962 Adding en entry to the DiploCorner menu]
* [http://forums.civfanatics.com/showthread.php?t=399743 UI: an introduction]
* [http://forums.civfanatics.com/showthread.php?t=461552 UI: a complete guide]
|}


= API =
[[Global Functions (Civ5)|Global Functions]]

== Objects ==
{|cellspacing="0" cellpadding="0"
|-
|'''Static objects'''
|
:'''Instances'''
|
:'''Data'''
|
:'''Events'''
|-
|valign="top" width="160"|
* {{Type5|ContentManager}}
* {{Type5|Game}}
* {{Type5|Locale}}
* {{Type5|Map}}
* {{Type5|Matchmaking}}
* {{Type5|Modding}}
* {{Type5|Network}}
* {{Type5|OptionsManager}}
* {{Type5|Path}}
* {{Type5|PreGame}}
* {{Type5|Steam}}
* {{Type5|TTManager}}
* {{Type5|UI}}
* {{Type5|UIManager}}
|valign="top" width="160"|
* {{Type5|Area}}
* {{Type5|City}}
* {{Type5|Deal}}
* {{Type5|Fractal}}
* {{Type5|Player}}
* {{Type5|Plot}}
* {{Type5|Team}}
* {{Type5|TeamTechs}}
* {{Type5|Unit}}
|valign="top" width="160"|
* {{Type5|ArtInfo}}
* {{Type5|DB}}
* {{Type5|GameDefines}}
* {{Type5|GameInfo}}
* {{Type5|GameInfoActions}}
* {{Type5|GameInfoTypes}}
|valign="top" width="160"|
* {{Type5|Events}}
* {{Type5|GameEvents}}
* {{Type5|LuaEvents}}
|}


== UI Controls ==
See also [[Common UI Properties (Civ5)|Common UI Properties]].
{|cellspacing="0" cellpadding="0"
|-
|
:'''Miscalleneous'''
|
:'''Buttons'''
|
:'''Containers'''
|
:'''Animations'''
|-
|valign="top" width="160"|
* {{Type5|Bar}}
* {{Type5|Context}}
* {{Type5|EditBox}}
* {{Type5|Image}}
* {{Type5|Instance}}
* {{Type5|Label}}
* {{Type5|Line}}
* {{Type5|Meter}}
* {{Type5|PullDown}}
* {{Type5|ReplayMap}}
* {{Type5|ScrollBar}}
* {{Type5|Shuttle}}
* {{Type5|Slider}}
* {{Type5|TextureBar}}
* {{Type5|ToolTipType}}
|valign="top" width="160"|
* {{Type5|BoxButton}}
* {{Type5|Button}}
* {{Type5|CheckBox}}
* {{Type5|DownButton}}
* {{Type5|GridButton}}
* {{Type5|RadioButton}}
* {{Type5|TextButton}}
* {{Type5|UpButton}}
|valign="top" width="160"|
* {{Type5|Box}}
* {{Type5|Container}}
* {{Type5|Grid}}
* {{Type5|ScrollPanel}}
* {{Type5|ShowOnMouseOver}}
* {{Type5|Stack}}
* {{Type5|WorldAnchor}}
|valign="top" width="160"|
* {{Type5|AlphaAnim}}
* {{Type5|FlipAnim}}
* {{Type5|ScrollAnim}}
* {{Type5|SlideAnim}}
|}


== Lua Objects ==
Those objects are defined in Lua files and can be used through an <code>include</code> statement.
{|cellspacing="0" cellpadding="0"
|-
|width="160"|
|width="160"|
|-
|valign="top"|
*{{Type5|AssignStartingPlots}}
*{{Type5|FeatureGenerator}}
*{{Type5|FractalWorld}}
*{{Type5|GameplayUtilities}}
|valign="top"|
*{{Type5|GenerationalInstanceManager}}
*{{Type5|InstanceManager}}
*{{Type5|MultilayeredFractal}}
*{{Type5|TerrainGenerator}}
|}


== Structures ==
Those objects are regular Lua tables that only contain named fields but no methods.
{|cellspacing="0" cellpadding="0"
|-
|width="160"|
|width="160"|
|width="160"|
|-
|valign="top"|
*{{Type5|ActionInfo}}
*{{Type5|AdvisorEventInfo}}
*{{Type5|CityEspionageInfo}}
*{{Type5|Color}}
*{{Type5|FileHeader}}
*{{Type5|IntrigueInfo}}
|valign="top"|
*{{Type5|MapFileInfo}}
*{{Type5|MapScriptInfo}}
*{{Type5|MapScriptOption}}
*{{Type5|MapScriptOptionValue}}
*{{Type5|ModDependency}}
*{{Type5|ModInfo}}
|valign="top"|
*{{Type5|MultiplayerGame}}
*{{Type5|OverlayInfo}}
*{{Type5|PopupInfo}}
*{{Type5|ReplayInfo}}
*{{Type5|ScenarioInfo}}
*{{Type5|SpyInfo}}
|valign="top"|
*{{Type5|TaskListInfo}}
*{{Type5|Vector2}}
*{{Type5|Vector3}}
*{{Type5|Vector4}}
*{{Type5|WorldBuilderMapData}}
|}


== Objects identifiers ==
Those identifiers are regular integers that identify objects.
{|cellspacing="0" cellpadding="0"
|-
|valign="top" width="160"|
* {{Type5|AreaID}}
* {{Type5|CityID}}
* {{Type5|CityPlotID}}
* {{Type5|MapOptionID}}
* {{Type5|PlotID}}
* {{Type5|UnitID}}
|valign="top"|
* {{Type5|PlayerID}} (<code>Players</code> enumeration)
* {{Type5|TeamID}} (<code>Teams</code> enumeration)
|}


== Constants identifiers ==
Those identifiers are regular integers associated with the constants defined in Lua enumerations.
{|cellspacing="0" cellpadding="0"
|-
|width="160"|
:'''Type'''
|width="160"|
:'''Lua Enum'''
|width="160"|
|width="170"|
:'''Type'''
|width="160"|
:'''Lua Enum'''
|-
|
*{{Type5|ActionSubType}}
|<code>ActionSubTypes</code>
|
|
*{{Type5|GameType}}
|<code>GameTypes</code>
|-
|
*{{Type5|ActivityType}}
|<code>ActivityTypes</code>
|
|
*{{Type5|GenericWorldAnchorType}}
|<code>GenericWorldAnchorTypes</code>
|-
|
*{{Type5|AdvisorType}}
|<code>AdvisorTypes</code>
|
|
*{{Type5|InfoCornerID}}
|<code>InfoCornerID</code>
|-
|
*{{Type5|ButtonPopupType}}
|<code>ButtonPopupTypes</code>
|
|
*{{Type5|InterfaceDirtyBits}}
|<code>InterfaceDirtyBits</code>
|-
|
*{{Type5|ButtonState}}
|<code>ButtonStates</code>
|
|
*{{Type5|KeyEventType}}
|<code>KeyEvents</code>
|-
|
*{{Type5|ChatTargetType}}
|<code>ChatTargetTypes</code>
|
|
*{{Type5|KeyType}}
|<code>Keys</code>
|-
|
*{{Type5|CityAIFocusType}}
|<code>CityAIFocusTypes</code>
|
|
*{{Type5|LeaderAnimationType}}
|<code>LeaderheadAnimationTypes</code>
|-
|
*{{Type5|CityUpdateType}}
|<code>CityUpdateTypes</code>
|
|
*{{Type5|MajorCivApproachType}}
|<code>MajorCivApproachTypes</code>
|-
|
*{{Type5|CombatPredictionType}}
|<code>CombatPredictionTypes</code>
|
|
*{{Type5|MinorCivPersonalityType}}
|<code>MinorCivPersonalityTypes</code>
|-
|
*{{Type5|CommandType}}
|<code>CommandTypes</code>
|
|
*{{Type5|MinorCivQuestType}}
|<code>MinorCivQuestTypes</code>
|-
|
*{{Type5|ContentType}}
|<code>ContentType</code>
|
|
*{{Type5|MouseEventType}}
|<code>MouseEvents</code>
|-
|
*{{Type5|ControlType}}
|<code>ControlTypes</code>
|
|
*{{Type5|MouseType}}
|<code>Mouse</code>
|-
|
*{{Type5|CoopWarState}}
|<code>CoopWarStates</code>
|
|
*{{Type5|NetError}}
|<code>NetErrors</code>
|-
|
*{{Type5|DiploUIEventType}}
|<code>FromUIDiploEventTypes</code>
|
|
*{{Type5|NetKicked}}
|<code>NetKicked</code>
|-
|
*{{Type5|DiploUIStateType}}
|<code>DiploUIStateTypes</code>
|
|
*{{Type5|OrderType}}
|<code>OrderTypes</code>
|-
|
*{{Type5|DirectionType}}
|<code>DirectionTypes</code>
|
|
*{{Type5|PlotType}}
|<code>PlotTypes</code>
|-
|
*{{Type5|DisputeLevelType}}
|<code>DisputeLevelTypes</code>
|
|
*{{Type5|PopupPriority}}
|<code>PopupPriority</code>
|-
|
*{{Type5|EndGameType}}
|<code>EndGameTypes</code>
|
|
*{{Type5|ResourceUsageType}}
|<code>ResourceUsageTypes</code>
|-
|
*{{Type5|EndTurnBlockingType}}
|<code>EndTurnBlockingTypes</code>
|
|
*{{Type5|SlotClaim}}
|<code>SlotClaim</code>
|-
|
*{{Type5|FaithPurchaseType}}
|<code>FaithPurchaseTypes</code>
|
|
*{{Type5|SlotStatus}}
|<code>SlotStatus</code>
|-
|
*{{Type5|FlowDirectionType}}
|<code>FlowDirectionTypes</code>
|
|
*{{Type5|SystemUpdateUIType}}
|<code>SystemUpdateUIType</code>
|-
|
*{{Type5|FogOfWarModeType}}
|<code>FogOfWarModeTypes</code>
|
|
*{{Type5|TaskType}}
|<code>TaskTypes</code>
|-
|
*{{Type5|GameMessageType}}
|<code>GameMessageTypes</code>
|
|
*{{Type5|ThreatType}}
|<code>ThreatTypes</code>
|-
|
*{{Type5|GameOptionType}}
|<code>GameOptionTypes</code>
|
|
*{{Type5|TradeableItemType}}
|<code>TradeableItems</code>
|-
|
*{{Type5|GameplayStateType}}
|<code>GameplayGameStateTypes</code>
|
|
*{{Type5|YieldDisplayType}}
|<code>YieldDisplayTypes</code>
|-
|
*{{Type5|GameStateType}}
|<code>GameStateTypes</code>
|
|}


== Data identifiers ==
Those identifiers are regular integers that identify the data rows defined in the XML data files.
{|cellspacing="0" cellpadding="0"
|-
|width="160"|
:'''Type'''
|width="200"|
:'''Xml Table'''
|width="160"|
:'''Lua Enum'''
|-
|
* {{Type5|ActionType}}
|{{Table5|Commands|CIV5Commands}}
|
|-
|
* {{Type5|ArtStyleType}}
|{{Table5|ArtStyleTypes|CIV5ArtStyleTypes}}
|
|-
|
* {{Type5|AutomateType}}
|{{Table5|Automates|CIV5Automates}}
|
|-
|
* {{Type5|BeliefType}}
|{{Table5|Beliefs|CIV5Beliefs}}
|<code>BeliefTypes</code>
|-
|
* {{Type5|BuildActionType}}
|{{Table5|Builds|CIV5Builds}}
|
|-
|
* {{Type5|BuildingClassType}}
|{{Table5|BuildingClasses|CIV5BuildingClasses}}
|
|-
|
* {{Type5|BuildingType}}
|{{Table5|Buildings|CIV5Buildings}}
|
|-
|
* {{Type5|CalendarType}}
|{{Table5|Calendars|CIV5Calendars}}
|
|-
|
* {{Type5|CivilizationType}}
|{{Table5|Civilizations|CIV5Civilizations}}
|
|-
|
* {{Type5|ClimateType}}
|{{Table5|Climates|CIV5Climates}}
|
|-
|
* {{Type5|ColorType}}
|{{Table5|Colors|CIV5Colors}}
|
|-
|
* {{Type5|DiploResponseType}}
|{{Table5|Diplomacy_Responses|CIV5Diplomacy_Responses}}
|
|-
|
* {{Type5|DomainType}}
|{{Table5|Domains|CIV5Domains}}
|<code>DomainTypes</code>
|-
|
* {{Type5|EraType}}
|{{Table5|Eras|CIV5Eras}}
|
|-
|
* {{Type5|FeatureType}}
|{{Table5|Features|CIV5Features}}
|<code>FeatureTypes</code>
|-
|
* {{Type5|FlavorType}}
|{{Table5|Flavors|CIV5Flavors}}
|
|-
|
* {{Type5|GameSpeedType}}
|{{Table5|GameSpeeds|CIV5GameSpeeds}}
|
|-
|
* {{Type5|GoodyType}}
|{{Table5|GoodyHuts|CIV5GoodyHuts}}
|
|-
|
* {{Type5|HandicapType}}
|{{Table5|HandicapInfos|CIV5HandicapInfos}}
|
|-
|
* {{Type5|HurryType}}
|{{Table5|HurryInfos|CIV5HurryInfos}}
|
|-
|
* {{Type5|ImprovementType}}
|{{Table5|Improvements|CIV5Improvements}}
|
|-
|
* {{Type5|InterfaceMode}}
|{{Table5|InterfaceModes|CIV5InterfaceModes}}
|<code>InterfaceModeTypes</code>
|-
|
* {{Type5|InvisibilityScopeType}}
|{{Table5|InvisibleInfos|CIV5InvisibleInfos}}
|
|-
|
* {{Type5|LeaderType}}
|{{Table5|Civilization_Leaders|CIV5Civilizations}}
|
|-
|
* {{Type5|MinorCivTraitType}}
|{{Table5|MinorCivTraits|CIV5MinorCivTraits}}
|<code>MinorCivTraitTypes</code>
|-
|
* {{Type5|MissionType}}
|{{Table5|Missions|CIV5Missions}}
|<code>MissionTypes</code>
|-
|
* {{Type5|MultiOptionType}}
|{{Table5|MultiplayerOptions|CIV5MultiplayerOptions}}
|
|-
|
* {{Type5|NotificationType}}
|{{Table5|Notifications|Notifications}}
|<code>NotificationTypes</code>
|-
|
* {{Type5|PlayerOptionType}}
|{{Table5|PlayerOptions|CIV5PlayerOptions}}
|
|-
|
* {{Type5|PolicyBranchType}}
|{{Table5|PolicyBranchTypes|CIV5PolicyBranchTypes}}
|<code>PolicyBranchTypes</code>
|-
|
* {{Type5|PolicyType}}
|{{Table5|Policies|CIV5Policies}}
|
|-
|
* {{Type5|ProcessType}}
|{{Table5|Processes|CIV5Processes}}
|
|-
|
* {{Type5|ProjectType}}
|{{Table5|Projects|CIV5Projects}}
|
|-
|
* {{Type5|PromotionType}}
|{{Table5|UnitPromotions|CIV5UnitPromotions}}
|
|-
|
* {{Type5|ReligionType}}
|{{Table5|Religions|CIV5Religions}}
|<code>ReligionTypes</code>
|-
|
* {{Type5|ReplayMessageType}}
|{{Table5|ReplayDataSets|CIV5Replays}}
|
|-
|
* {{Type5|ResourceType}}
|{{Table5|Resources|CIV5Resources}}
|
|-
|
* {{Type5|RouteType}}
|{{Table5|Routes|CIV5Routes}}
|
|-
|
* {{Type5|SpecialistType}}
|{{Table5|Specialists|CIV5Specialists}}
|
|-
|
* {{Type5|SpecialUnitType}}
|{{Table5|SpecialUnits|CIV5SpecialUnits}}
|
|-
|
* {{Type5|TechType}}
|{{Table5|Technologies|CIV5Technologies}}
|
|-
|
* {{Type5|TerrainType}}
|{{Table5|Terrains|CIV5Terrains}}
|<code>TerrainTypes</code>
|-
|
* {{Type5|UnitAIType}}
|{{Table5|UnitAIInfos|CIV5UnitAIInfos}}
|
|-
|
* {{Type5|UnitClassType}}
|{{Table5|UnitClasses|CIV5UnitClasses}}
|
|-
|
* {{Type5|UnitCombatType}}
|{{Table5|UnitCombatInfos|CIV5UnitCombatInfos}}
|
|-
|
* {{Type5|UnitType}}
|{{Table5|Units|CIV5Units}}
|
|-
|
* {{Type5|VictoryType}}
|{{Table5|Victories|CIV5Victories}}
|
|-
|
* {{Type5|VoteSourceType}}
|{{Table5|VoteSources|CIV5VoteSources}}
|
|-
|
* {{Type5|VoteType}}
|{{Table5|Votes|CIV5Votes}}
|
|-
|
* {{Type5|YieldType}}
|{{Table5|Yields|CIV5Yields}}
|<code>YieldTypes</code>
|}


= Categories =
[[:Category:Civ5 API|Civ5 API]]
:[[:Category:Civ5 Types|Civ5 Types]]
:[[:Category:Civ5 Methods and Functions|Civ5 Methods and Functions]]
:[[:Category:Civ5 Thematic Categories: Terrain|Civ5 Thematic Categories: Terrain]]
::[[:Category:Civ5 Features & Natural wonders API|Civ5 Features & Natural wonders API]]
::[[:Category:Civ5 Fog API|Civ5 Fog API]]
::[[:Category:Civ5 Goodies API|Civ5 Goodies API]]
::[[:Category:Civ5 Improvements API|Civ5 Improvements API]]
::[[:Category:Civ5 Resources API|Civ5 Resources API]]
::[[:Category:Civ5 Rivers API|Civ5 Rivers API]]
::[[:Category:Civ5 Terrain API|Civ5 Terrain API]]
::[[:Category:Civ5 Terrain Ownership API|Civ5 Terrain Ownership API]]
::[[:Category:Civ5 Yields API|Civ5 Yields API]]
:[[:Category:Civ5 Thematic Categories: Development|Civ5 Thematic Categories: Development]]
::[[:Category:Civ5 Buildings API|Civ5 Buildings API]]
::[[:Category:Civ5 Cities API|Civ5 Cities API]]
::[[:Category:Civ5 City Production API|Civ5 City Production API]]
::[[:Category:Civ5 Culture API|Civ5 Culture API]]
::[[:Category:Civ5 Food & Population API|Civ5 Food & Population API]]
::[[:Category:Civ5 Gold API|Civ5 Gold API]]
::[[:Category:Civ5 Golden Age API|Civ5 Golden Age API]]
::[[:Category:Civ5 Great People API|Civ5 Great People API]]
::[[:Category:Civ5 Happiness API|Civ5 Happiness API]]
::[[:Category:Civ5 Policies API|Civ5 Policies API]]
::[[:Category:Civ5 Religion API|Civ5 Religion API]]
::[[:Category:Civ5 Science API|Civ5 Science API]]
::[[:Category:Civ5 Specialists API|Civ5 Specialists API]]
:[[:Category:Civ5 Thematic Categories: Units|Civ5 Thematic Categories: Units]]
::[[:Category:Civ5 Barbarians API|Civ5 Barbarians API]]
::[[:Category:Civ5 Combat API|Civ5 Combat API]]
::[[:Category:Civ5 Movement API|Civ5 Movement API]]
::[[:Category:Civ5 Unit Experience API|Civ5 Unit Experience API]]
::[[:Category:Civ5 Units API|Civ5 Units API]]
:[[:Category:Civ5 Thematic Categories: Diplomacy|Civ5 Thematic Categories: Diplomacy]]
::[[:Category:Civ5 City States API|Civ5 City States API]]
::[[:Category:Civ5 Diplomacy API|Civ5 Diplomacy API]]
::[[:Category:Civ5 Espionnage API|Civ5 Espionnage API]]
::[[:Category:Civ5 Players API|Civ5 Players API]]
::[[:Category:Civ5 Trade API|Civ5 Trade API]]
::[[:Category:Civ5 United Nations API|Civ5 United Nations API]]
:[[:Category:Civ5 Thematic Categories: General|Civ5 Thematic Categories: General]]
::[[:Category:Civ5 Game Settings API|Civ5 Game Settings API]]
::[[:Category:Civ5 Notification API|Civ5 Notification API]]
::[[:Category:Civ5 Score API|Civ5 Score API]]
::[[:Category:Civ5 Turns API|Civ5 Turns API]]
::[[:Category:Civ5 Victory API|Civ5 Victory API]]


= Contributing =
* [[Contributors guide to the Civ5 API]]
* [[:Category:Civ5 API Templates]]
* [[:Category:Civ5 API Images]]


{{Civ5 API Footer}}
[[Category:Civ5 API]]
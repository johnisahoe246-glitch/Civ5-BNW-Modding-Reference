The '''GlobalDefines''' file defines various properties of the game.  Mods can use the '''GlobalDefinesAlt''' file as a modular way to only include defines that have been changed.  Each define only have one of the non-header tags.

All tags must be opened and closed; the first is the "open", the second the "close" tag. If nothing goes inside a "list tag", then it should just be the opening tag with a "/" before the closing bracket. The following tables contain all available tags, as well as their purpose and accepted values. 

<font color=red>This page is missing information.
Do not remove this notice until it is complete.</font>


==Tags==
===Headers===

These tags typically bracket other tags, sometimes the entire file, and are generally used to specify more than one piece of data.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Define
|Main bracket for each entry
|-
!DefineName
|Name used in other files
|}


===Text===

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!DefineTextVal
|Text value of the define; often refers to other XML entires
|}


===Integers===

All of these tags have a numerical value.  Though it sometimes can be negative, it usually is not.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!iDefineIntVal
|Integer value for the define
|}


===Floats===

All of these tags have a decimal value.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!fDefineFloatVal
|Floating point value for a define
|}


==Example==

In the following example of code, please note that there is a specific order of all of the tags.  You ''must'' list the tags in this order for the game to properly interpret your file.

 <Define>
  <DefineName>NUKE_FEATURE</DefineName>
  <DefineTextVal>FEATURE_FALLOUT</DefineTextVal>
 </Define>


==The Defines==

The following is a list of the defines in the file.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Define Name
! style="background:#efefef;" | Description
|-
!CIV4_VERSION
|Version of civ4 used in the About screen on the main menu
|-
!MIN_VERSION
|Minimum version of civ4 a mod requires to run
|-
!SAVE_VERSION
|Last version of civ4 to break save game compatability
|-
!MAX_NUM_LANGUAGES
|Maximum number of languages that can be supported by the game
|-
!LAND_TERRAIN
|Default type of terrain used for land when generating the map
|-
!DEEP_WATER_TERRAIN
|Default type of terrain used for deep water when generating the map
|-
!SHALLOW_WATER_TERRAIN
|Default type of terrain used for shallow water when generating the map
|-
!LAND_IMPROVEMENT
|Improvement used to mark worked tile on land
|-
!WATER_IMPROVEMENT
|Improvement used to mark worked tile on water
|-
!RUINS_IMPROVEMENT
|Improvement used for city ruins
|-
!NUKE_FEATURE
|Feature used for nuclear fallout
|-
!GLOBAL_WARMING_TERRAIN
|Terrain used for global warming
|-
!CAPITAL_BUILDINGCLASS
|Buildingclass used to designate which city is the capital
|-
!DEFAULT_SPECIALIST
|Specialist allocated by default by city AI
|-
!INITIAL_CITY_ROUTE_TYPE
|Initial route placed on tiles cities are founded on
|-
!STANDARD_HANDICAP
|Default difficulty level
|-
!STANDARD_HANDICAP_QUICK
|Default difficulty level on quick game speed
|-
!STANDARD_GAMESPEED
|Default game speed
|-
!STANDARD_TURNTIMER
|Default turn timer used in multiplayer
|-
!STANDARD_CLIMATE
|Default climate
|-
!STANDARD_SEALEVEL
|Default sea level
|-
!STANDARD_ERA
|Default starting era
|-
!STANDARD_CALENDAR
|Default calendar
|-
!AI_HANDICAP
|Difficulty level used by the AI
|-
!BARBARIAN_HANDICAP
|Difficulty level used by the barbarians
|-
!BARBARIAN_CIVILIZATION
|Civilization used by the barbarians
|-
!BARBARIAN_LEADER
|Leader used by the barbarians
|-
!MAX_PLOT_LIST_SIZE
|Unknown
|-
!MAX_PLOT_LIST_ROWS
|Unknown
|-
!EVENT_MESSAGE_TIME
|Time (in seconds) messages are displayed by the game
|-
!EVENT_MESSAGE_TIME_LONG
|Unknown
|-
!EVENT_MESSAGE_STAGGER_TIME
|Time (in seconds) before another message can be displayed
|-
!START_YEAR
|Default starting year
|-
!WEEKS_PER_MONTHS
|Number of weeks in a month; used for the weekly calendar
|-
!TERRAIN_POINTS
|Number of points per terrain tile controlled
|-
!RECON_VISIBILITY_RANGE
|Unknown
|-
!PLOT_VISIBILITY_RANGE
|Unknown
|-
!UNIT_VISIBILITY_RANGE
|Unknown
|-
!PEAK_SEE_FROM_CHANGE
|Additional tile radius of visibility given to unit on a peak
|-
!PEAK_SEE_THROUGH_CHANGE
|Additional tile radius of visibility removed from unit where tile visibility is blocked by a peak
|-
!HILLS_SEE_FROM_CHANGE
|Additional tile radius of visibility given to unit on a hill
|-
!HILLS_SEE_THROUGH_CHANGE
|Additional tile radius of visibility removed from unit where tile visibility is blocked by a hill
|-
!SEAWATER_SEE_FROM_CHANGE
|Additional tile radius of visibility given to unit on sea water
|-
!SEAWATER_SEE_THROUGH_CHANGE
|Additional tile radius of visibility removed from unit where tile visibility is blocked by sea water
|-
!RAND_YIELD_PRESENCE_DIE_ROLLS
|Unknown
|-
!MAX_YIELD_STACK
|Unknown
|-
!MOVE_DENOMINATOR
|Unknown
|-
!STARTING_DISTANCE_PERCENT
|Unknown
|-
!OWN_TEAM_STARTING_MODIFIER
|Unknown
|-
!RIVAL_TEAM_STARTING_MODIFIER
|Unknown
|-
!MIN_CIV_STARTING_DISTANCE
|Minimum distance in starting locations between civilizations the game tries to uphold
|-
!MIN_ANIMAL_STARTING_DISTANCE
|Minimum distance from a civilization an animal can spawn on
|-
!MIN_BARBARIAN_STARTING_DISTANCE
|Minimum distance from a civilization a barbarian can spawn on
|-
!MIN_BARBARIAN_CITY_STARTING_DISTANCE
|Minimum distance from a civilization a barbarian city can spawn on
|-
!MIN_CITY_RANGE
|Minimum distance between cities
|-
!FREE_CITY_CULTURE
|Unknown
|-
!FREE_CITY_ADJACENT_CULTURE
|Unknown
|-
!CITY_FREE_CULTURE_GROWTH_FACTOR
|Unknown
|-
!GREAT_WORKS_CULTURE_TURNS
|Unknown
|-
!OWNERSHIP_SCORE_DURATION_THRESHOLD
|Unknown
|-
!NUM_DO_GOODY_ATTEMPTS
|Number of times the game can attempt to get something from a tribal village before giving up (ie, giving the player nothing from the tribal village)
|-
!MAX_CIVIC_OPTIONS
|Max number of civics that can be in a civic category
|-
!BASE_CIVIC_ANARCHY_LENGTH
|Minimum length of anarchy for civic changes
|-
!BASE_RELIGION_ANARCHY_LENGTH
|Length of anarchy for changing religions
|-
!COMMERCE_PERCENT_CHANGE_INCREMENTS
|Percent change in slider allocation for commerce types the user can change with the interface
|-
!INITIAL_TRADE_ROUTES
|Initial number of trade routes per city
|-
!NUM_OR_TECH_PREREQS
|Number of or tech prereqs a tech can have
|-
!MAX_AND_TECH_PREREQS
|Number of and tech prereqs a tech can have
|-
!NUM_UNIT_AND_TECH_PREREQS
|Number of and tech prereqs a unit can have
|-
!NUM_BUILDING_AND_TECH_PREREQS
|Number of and tech prereqs a building can have
|-
!BASE_RESEARCH_RATE
|Unknown
|-
!NUM_UNIT_PREREQ_OR_BONUSES
|Number of or resource prereqs a unit can have
|-
!NUM_CORPORATION_PREREQ_BONUSES
|Number of prereq resources a corporation can have
|-
!NUM_ROUTE_PREREQ_OR_BONUSES
|Number of or prereq resources a route can have
|-
!MAX_WORLD_WONDERS_PER_CITY
|Highest number of world wonders a city can have
|-
!MAX_TEAM_WONDERS_PER_CITY
|Highest number of team wonders a city can have
|-
!MAX_NATIONAL_WONDERS_PER_CITY
|Highest number of national wonders a city can have
|-
!MAX_NATIONAL_WONDERS_PER_CITY_FOR_OCC
|Highest number of national wonders a city can have in a one city challenge game
|-
!MAX_BUILDINGS_PER_CITY
|Highest number of buildings a city can have
|-
!INITIAL_CITY_POPULATION
|Initial population for newly founded cities
|-
!INITIAL_AI_CITY_PRODUCTION
|Unknown
|-
!BASE_CITY_GROWTH_THRESHOLD
|Base amount of food a city needs to growth
|-
!CITY_GROWTH_MULTIPLIER
|Multiplier for additional amount of food needed for each time a city gains a population point
|-
!FOOD_CONSUMPTION_PER_POPULATION
|Amount of food each population point consumes
|-
!NEW_HURRY_MODIFIER
|Unknown
|-
!CONSCRIPT_MIN_CITY_POPULATION
|Minimum population in a city needed to draft a unit
|-
!CONSCRIPT_POPULATION_PER_COST
|Unknown
|-
!CONSCRIPT_MIN_CULTURE_PERCENT
|Minimum percentage of city culture that has to be your own to draft a unit
|-
!FRESH_WATER_HEALTH_CHANGE
|Amount of health added to city from being near fresh water
|-
!POWER_HEALTH_CHANGE
|Health change from having power
|-
!DIRTY_POWER_HEALTH_CHANGE
|Health change from dirty power
|-
!INITIAL_CITY_MAINTENANCE
|Maintenance cost for the first city
|-
!MAX_DISTANCE_CITY_MAINTENANCE
|Maximum city maintenance from distance
|-
!MAX_TRADE_ROUTES
|Maximum number of trade routes a city can have
|-
!MIN_TIMER_UNIT_DOUBLE_MOVES
|Unknown
|-
!DYING_PAUSE
|Unknown
|-
!COMBAT_DAMAGE
|Unknown
|-
!AIR_COMBAT_DAMAGE
|Unknown
|-
!INTERCEPTION_MAX_ROUNDS
|Maximum number of combat rounds when aircraft intercepted
|-
!MAX_INTERCEPTION_DAMAGE
|Maximum amount of damage done to intercepted aircraft
|-
!MIN_INTERCEPTION_DAMAGE
|Minimum amount of damage done to intercepted aircraft
|-
!RANGE_COMBAT_DAMAGE
|Unknown
|-
!COLLATERAL_COMBAT_DAMAGE
|Unknown
|-
!MAX_HIT_POINTS
|Maximum number of hit points a unit can have
|-
!COMBAT_DIE_SIDES
|Unknown
|-
!HILLS_EXTRA_DEFENSE
|Defensive bonus from being on hills
|-
!RIVER_ATTACK_MODIFIER
|Penalty for attacking across a river
|-
!AMPHIB_ATTACK_MODIFIER
|Penalty for attacking from a transport
|-
!ENEMY_HEAL_RATE
|Rate of healing in enemy territory
|-
!NEUTRAL_HEAL_RATE
|Rate of healing in neutral territory
|-
!FRIENDLY_HEAL_RATE
|Rate of healing in team territory
|-
!CITY_HEAL_RATE
|Rate of healing in city
|-
!FOUND_RELIGION_CITY_RAND
|Unknown
|-
!FOUND_CORPORATION_CITY_RAND
|Unknown
|-
!GREAT_PEOPLE_THRESHOLD_INCREASE
|Increase in great people points needed for each additional great person in civilization
|-
!GREAT_PEOPLE_THRESHOLD_INCREASE_TEAM
|Increase in great people points needed for each additional great person in team
|-
!GREAT_PEOPLE_THRESHOLD
|Initial number of great person points needed for great person
|-
!GREAT_GENERALS_THRESHOLD_INCREASE
|Increase in number of great general points needed for each additional great general in civilization
|-
!GREAT_GENERALS_THRESHOLD_INCREASE_TEAM
|Increase in number of great general points needed for each additional great general in team
|-
!GREAT_GENERALS_THRESHOLD
|Initial number of great general points needed for great general
|-
!BASE_SPY_SABOTAGE_COST
|Base cost for non-BtS sabotage production spy mission
|-
!BASE_SPY_DESTROY_COST
|Base cost for non-BtS destroy improvement spy mission
|-
!SPY_DESTROY_COST_MULTIPLIER_LIMITED
|Unknown
|-
!SPY_DESTROY_COST_MULTIPLIER
|Cost increase for non-BtS destroy improvement spy mission
|-
!BASE_SPY_STEAL_PLANS_COST
|Base cost for non-BtS steal plans spy mission
|-
!SPY_STEAL_PLANS_COST_MULTIPLIER
|Cost increase for non-BtS steal plans mission
|-
!QUICKSAVE
|Text name for QuickSave
|-
!LAKE_PLOT_RAND
|Unknown
|-
!PLOTS_PER_RIVER_EDGE
|Unknown
|-
!RIVER_SOURCE_MIN_RIVER_RANGE
|Unknown
|-
!RIVER_SOURCE_MIN_SEAWATER_RANGE
|Unknown
|-
!LAKE_MAX_AREA_SIZE
|Unknown
|-
!INITIAL_BASE_FREE_UNITS
|Base number of free units
|-
!INITIAL_BASE_FREE_MILITARY_UNITS
|Base number of free military units
|-
!INITIAL_FREE_UNITS_POPULATION_PERCENT
|Unknown
|-
!INITIAL_FREE_MILITARY_UNITS_POPULATION_PERCENT
|Unknown
|-
!INITIAL_GOLD_PER_UNIT
|Initial maintenance cost per unit
|-
!INITIAL_FREE_OUTSIDE_UNITS
|Initial number of free units outside the civilization
|-
!INITIAL_OUTSIDE_UNIT_GOLD_PERCENT
|Unknown
|-
!ANIMAL_MAX_XP_VALUE
|Maximum amount of XP a unit can have before not getting XP from animals
|-
!BARBARIAN_MAX_XP_VALUE
|Maximum amount of XP a unit can have before not getting XP from barbarians
|-
!BASE_GOLDEN_AGE_UNITS
|Base number of great people needed to start a golden age
|-
!GOLDEN_AGE_UNITS_MULTIPLIER
|Additional number of great people needed to start each golden age
|-
!GOLDEN_AGE_LENGTH
|Length of golden ages
|-
!GOLDEN_AGE_GREAT_PEOPLE_MODIFIER
|Percent increase in great people points in golden age
|-
!HILLS_EXTRA_MOVEMENT
|Extra movement points needed when moving onto a hill
|-
!FEATURE_GROWTH_MODIFIER
|Unknown
|-
!ROUTE_FEATURE_GROWTH_MODIFIER
|Percent decrease in feature growth on tiles with a route
|-
!THEIR_POPULATION_TRADE_PERCENT
|Unknown
|-
!CAPITAL_TRADE_MODIFIER
|Percent increase in trade yield from capital cities
|-
!OVERSEAS_TRADE_MODIFIER
|Percent increase in trade yield from overseas cities
|-
!FOREIGN_TRADE_MODIFIER
|Percent increase in trade yield from foreign cities
|-
!FOREIGN_TRADE_FULL_CREDIT_PEACE_TURNS
|Unknown
|-
!OUR_POPULATION_TRADE_MODIFIER
|Unknown
|-
!OUR_POPULATION_TRADE_MODIFIER_OFFSET
|Unknown
|-
!TRADE_PROFIT_PERCENT
|Unknown
|-
!EXTRA_YIELD
|Unknown
|-
!FORTIFY_MODIFIER_PER_TURN
|Percent defensive bonus applied each turn unit is fortified
|-
!MAX_FORTIFY_TURNS
|Maximum number of turns a unit can get an additional fortification defensive bonus
|-
!WW_UNIT_KILLED_ATTACKING
|War weariness from unit killed when attacking
|-
!WW_KILLED_UNIT_DEFENDING
|War weariness killing unit when defending
|-
!WW_UNIT_KILLED_DEFENDING
|War weariness from unit killed when defending
|-
!WW_KILLED_UNIT_ATTACKING
|War weariness killing unit when attacking
|-
!WW_UNIT_CAPTURED
|War weariness from unit captured
|-
!WW_CAPTURED_UNIT
|War weariness from capturing unit
|-
!WW_CAPTURED_CITY
|War weariness from captured city
|-
!WW_HIT_BY_NUKE
|War weariness from being hit by a nuke
|-
!WW_ATTACKED_WITH_NUKE
|War Weariness from using nuke
|-
!WW_DECAY_RATE
|Unknown
|-
!WW_DECAY_PEACE_PERCENT
|Unknown
|-
!NUKE_FALLOUT_PROB
|Percent chance a tile bordering a nuke attack gets fallout
|-
!NUKE_UNIT_DAMAGE_BASE
|Unknown
|-
!NUKE_UNIT_DAMAGE_RAND_1
|Unknown
|-
!NUKE_UNIT_DAMAGE_RAND_2
|Unknown
|-
!NUKE_NON_COMBAT_DEATH_THRESHOLD
|Unknown
|-
!NUKE_BUILDING_DESTRUCTION_PROB
|Percent chance for building to be destroyed by nuke
|-
!NUKE_POPULATION_DEATH_BASE
|Unknown
|-
!NUKE_POPULATION_DEATH_RAND_1
|Unknown
|-
!NUKE_POPULATION_DEATH_RAND_2
|Unknown
|-
!GLOBAL_WARMING_PROB
|Unknown
|-
!GLOBAL_WARMING_FOREST
|Unknown
|-
!GLOBAL_WARMING_UNHEALTH_WEIGHT
|Unknown
|-
!GLOBAL_WARMING_NUKE_WEIGHT
|Unknown
|-
!TECH_COST_EXTRA_TEAM_MEMBER_MODIFIER
|Unknown
|-
!TECH_COST_TOTAL_KNOWN_TEAM_MODIFIER
|Unknown
|-
!TECH_COST_KNOWN_PREREQ_MODIFIER
|Unknown
|-
!PEACE_TREATY_LENGTH
|Length of peace treaty
|-
!MAX_ANARCHY_TURNS
|Maximum number of turns for anarchy
|-
!MIN_REVOLUTION_TURNS
|Unknown
|-
!MIN_CONVERSION_TURNS
|Unknown
|-
!OCCUPATION_CULTURE_PERCENT_THRESHOLD
|Unknown
|-
!BASE_OCCUPATION_TURNS
|Unknown
|-
!OCCUPATION_TURNS_POPULATION_PERCENT
|Unknown
|-
!BASE_REVOLT_OCCUPATION_TURNS
|Unknown
|-
!REVOLT_OCCUPATION_TURNS_PERCENT
|Unknown
|-
!REVOLT_TOTAL_CULTURE_MODIFIER
|Unknown
|-
!REVOLT_OFFENSE_STATE_RELIGION_MODIFIER
|Unknown
|-
!REVOLT_DEFENSE_STATE_RELIGION_MODIFIER
|Unknown
|-
!REVOLT_TEST_PROB
|Unknown
|-
!NUM_WARNING_REVOLTS
|Number of revolts before a city culture flips
|-
!BASE_REVOLT_FREE_UNITS
|Unknown
|-
!REVOLT_FREE_UNITS_PERCENT
|Unknown
|-
!NO_MILITARY_PERCENT_ANGER
|Unknown
|-
!AT_WAR_CULTURE_ANGER_MODIFIER
|Unknown
|-
!CULTURE_PERCENT_ANGER
|Unknown
|-
!RELIGION_PERCENT_ANGER
|Unknown
|-
!HURRY_POP_ANGER
|Unknown
|-
!HURRY_ANGER_DIVISOR
|Unknown
|-
!CONSCRIPT_POP_ANGER
|Unknown
|-
!CONSCRIPT_ANGER_DIVISOR
|Unknown
|-
!DEFY_RESOLUTION_POP_ANGER
|Unknown
|-
!DEFY_RESOLUTION_ANGER_DIVISOR
|Unknown
|-
!TEMP_HAPPY
|Unknown
|-
!BASE_WAR_WEARINESS_MULTIPLIER
|Unknown
|-
!FORCED_WAR_WAR_WEARINESS_MODIFIER
|Unknown
|-
!MULTIPLAYER_WAR_WEARINESS_MODIFIER
|Unknown
|-
!PERCENT_ANGER_DIVISOR
|Unknown
|-
!BASE_FEATURE_PRODUCTION_PERCENT
|Unknown
|-
!FEATURE_PRODUCTION_PERCENT_MULTIPLIER
|Unknown
|-
!DIFFERENT_TEAM_FEATURE_PRODUCTION_PERCENT
|Unknown
|-
!UNIT_PRODUCTION_PERCENT
|Unknown
|-
!BUILDING_PRODUCTION_PERCENT
|Unknown
|-
!PROJECT_PRODUCTION_PERCENT
|Unknown
|-
!MAXED_UNIT_GOLD_PERCENT
|Unknown
|-
!MAXED_BUILDING_GOLD_PERCENT
|Unknown
|-
!MAXED_PROJECT_GOLD_PERCENT
|Unknown
|-
!MAX_CITY_DEFENSE_DAMAGE
|Unknown
|-
!CITY_DEFENSE_DAMAGE_HEAL_RATE
|Unknown
|-
!UPKEEP_POPULATION_OFFSET
|Unknown
|-
!UPKEEP_CITY_OFFSET
|Unknown
|-
!CIRCUMNAVIGATE_FREE_MOVES
|Free moves from circumnavigating the map
|-
!BARBARIAN_FREE_TECH_PERCENT
|Unknown
|-
!RAZING_CULTURAL_PERCENT_THRESHOLD
|Unknown
|-
!BASE_CAPTURE_GOLD
|Base amount of gold captured with city
|-
!CAPTURE_GOLD_PER_POPULATION
|Additional gold captured per population point
|-
!CAPTURE_GOLD_RAND1
|Unknown
|-
!CAPTURE_GOLD_RAND2
|Unknown
|-
!CAPTURE_GOLD_MAX_TURNS
|Unknown
|-
!CITY_BARBARIAN_DEFENSE_MODIFIER
|Unknown
|-
!MIN_EXPERIENCE_PER_COMBAT
|Minimum experience gained per combat
|-
!MAX_EXPERIENCE_PER_COMBAT
|Maximum experience gained per combat
|-
!EXPERIENCE_FROM_WITHDRAWL
|Experience gained when unit withdraws
|-
!MAX_EXPERIENCE_AFTER_UPGRADE
|Maximum experience a unit can retain when upgrading
|-
!BUILDING_PRODUCTION_DECAY_TIME
|Unknown
|-
!BUILDING_PRODUCTION_DECAY_PERCENT
|Unknown
|-
!UNIT_PRODUCTION_DECAY_TIME
|Unknown
|-
!UNIT_PRODUCTION_DECAY_PERCENT
|Unknown
|-
!BASE_UNIT_UPGRADE_COST
|Unknown
|-
!UNIT_UPGRADE_COST_PER_PRODUCTION
|Unknown
|-
!WAR_SUCCESS_DEFENDING
|Unknown
|-
!WAR_SUCCESS_ATTACKING
|Unknown
|-
!WAR_SUCCESS_UNIT_CAPTURING
|Unknown
|-
!WAR_SUCCESS_CITY_CAPTURING
|Unknown
|-
!WAR_SUCCESS_NUKE
|Unknown
|-
!GAME_CITY_SIZE_METHOD
|Method for computing visual city size; either METHOD_EXPONENTIAL or METHOD_LINMAP
|-
!GAME_CITY_SIZE_MAX_PERCENT_UNIQUE
|Percentage of a city that can be wonders
|-
!GAME_CITY_SIZE_EXP_MODIFIER
|Modifier to tweak city size when METHOD_EXPONENTIAL is chosen
|-
!GAME_CITY_SIZE_LINMAP_AT_0
|Visual size of city in METHOD_LINMAP at population 0
|-
!GAME_CITY_SIZE_LINMAP_AT_50
|Visual size of city in METHOD_LINMAP at population 50
|-
!DIPLO_VOTE_SECRETARY_GENERAL_INTERVAL
|Turn interval for UN and AP secretary general votes
|-
!TEAM_VOTE_MIN_CANDIDATES
|Minimum number of candidates for secretary general votes
|-
!DIPLOMACY_VALUE_REMAINDER
|Unknown
|-
!INITIAL_STATE_RELIGION_HAPPINESS
|Initial happiness from state relegion
|-
!INITIAL_NON_STATE_RELIGION_HAPPINESS
|Initial happiness from non-state religions
|-
!RELIGION_SPREAD_DISTANCE_DIVISOR
|Unknown
|-
!RELIGION_SPREAD_RAND
|Unknown
|-
!CORPORATION_FOREIGN_SPREAD_COST_PERCENT
|Unknown
|-
!HOLY_CITY_INFLUENCE
|Unknown
|-
!WE_LOVE_THE_KING_RAND
|Unknown
|-
!WE_LOVE_THE_KING_POPULATION_MIN_POPULATION
|Minimum population needed for a city to get the we love the king event
|-
!PLOT_SIZE
|Unknown
|-
!DISABLE_CLOSE_ZOOM_MODE
|Unknown
|-
!CAMERA_UPPER_PITCH
|Unknown
|-
!CAMERA_LOWER_PITCH
|Unknown
|-
!CAMERA_MIN_SCROLL_SPEED
|Unknown
|-
!CAMERA_MAX_SCROLL_SPEED
|Unknown
|-
!CAMERA_MIN_YAW
|Unknown
|-
!CAMERA_MAX_YAW
|Unknown
|-
!CAMERA_START_DISTANCE
|Unknown
|-
!CAMERA_MAX_TRAVEL_DISTANCE
|Unknown
|-
!CAMERA_MIN_DISTANCE
|Unknown
|-
!CAMERA_MAX_TURN_OFFSET
|Unknown
|-
!CAMERA_SMALLEST_MAX_DISTANCE
|Unknown
|-
!CAMERA_FORCE_TO_SMALLEST_MAX_DISTANCE
|Unknown
|-
!CAMERA_NEAR_FAR_PLANE_RATIO
|Unknown
|-
!ALLOW_UNIT_SCALE_ADJUST_ON_ZOOM
|Unknown
|-
!RENDER_AREABORDER_UNDER_FEATURES
|Unknown
|-
!RENDER_GLOBEVIEW_CLOUDS
|Unknown
|-
!RENDER_WATER
|Unknown
|-
!CAMERA_CITY_ZOOM_IN_DISTANCE
|Unknown
|-
!CAMERA_BATTLE_ZOOM_IN_DISTANCE
|Unknown
|-
!CAMERA_SHRINE_ZOOM_IN_DISTANCE
|Unknown
|-
!CAMERA_FAR_CLIP_Z_HEIGHT
|Unknown
|-
!EFFECT_DEFAULT_SIZE
|Unknown
|-
!UNIT_MULTISELECT_MAX
|Unknown
|-
!UNIT_MULTISELECT_SCALE
|Unknown
|-
!UNIT_MULTISELECT_DISTANCE
|Unknown
|-
!FIELD_OF_VIEW
|Unknown
|-
!IMPROVEMENT_SCALE
|Unknown
|-
!BONUS_SCALE
|Unknown
|-
!SHADOW_SCALE
|Unknown
|-
!HEALTH_BAR_WIDTH
|Unknown
|-
!AIR_IDLE_HEIGHT
|Height of an idling air unit
|-
!AIR_PATROL_RADIUS
|Relative radius of an air unit while patrolling
|-
!AIR_PATROL_SPEED
|Speed of air unit while patrolling
|-
!AIR_PATROL_HEIGHT
|Height of a patrolling air unit
|-
!AIR_BOMB_HEIGHT
|Height of a bombing air unit
|-
!AIR_EXECUTE_DISTANCE
|Distance an attacker/recon travels during an air mission (start to target)
|-
!AIR_EXECUTE_FINISH
|Distance an attacker/recon travels during an air mission (after target)
|-
!AIR_DEFEND_DISTANCE
|Distance a defender travels during an air mission (start to target)
|-
!AIR_DEFEND_FINISH
|Distance a defender travels during an air mission (after target)
|-
!UNIT_ANIM_PAGE_MAX
|Maximum number of animations loaded in memory for any unit
|-
!DEFAULT_ANIM_PAGE_MAX
|Default number of animations loaded for an entity
|-
!FLAG_OFFSET_X
|The relative offset X offset of a flag within a square (-1..1)
|-
!FLAG_OFFSET_Y
|The relative offset Y offset of a flag within a square (-1..1)
|-
!FLAG_OFFSET2_X
|The relative offset X offset of the second flag within a square (-1..1)
|-
!FLAG_OFFSET2_Y
|The relative offset Y offset of the second flag within a square (-1..1)
|-
!UNIT_TRAIL_RESOLUTION
|The resolution of the wake/trail left by units
|-
!SCORE_POPULATION_FACTOR
|Score you get if you have the 'maximum' population possible on the current map
|-
!SCORE_LAND_FACTOR
|Score you get if you have all the land on the current map
|-
!SCORE_WONDER_FACTOR
|Score you get if you have all the wonders
|-
!SCORE_TECH_FACTOR
|Score you get if you have all the techs
|-
!SCORE_FREE_PERCENT
|Percentage of the maximum score you get for free
|-
!SCORE_VICTORY_PERCENT
|Percentage of your score that gets added if you win the game
|-
!SCORE_HANDICAP_PERCENT_OFFSET
|Offset to the score handicap modifier
|-
!SCORE_HANDICAP_PERCENT_PER
|The amount of the score modifier per handicap level
|-
!MINIMAP_RENDER_SIZE
|Minimap size in pixels
|-
!TURN_LOG_MAX_WIDTH
|Unknown
|-
!TURN_LOG_MAX_HEIGHT
|Unknown
|-
!TURN_LOG_MIN_HEIGHT
|Unknown
|-
!LEADERHEAD_RANDOM
|Unknown
|-
!SINGLE_UNIT_GFX_EXTRA_SCALE
|Unknown
|-
!VASSAL_REVOLT_OWN_LOSSES_FACTOR
|Unknown
|-
!VASSAL_REVOLT_MASTER_LOSSES_FACTOR
|Unknown
|-
!VASSAL_HAPPINESS
|Unknown
|-
!FREE_VASSAL_LAND_PERCENT
|Unknown
|-
!FREE_VASSAL_POPULATION_PERCENT
|Unknown
|-
!WARLORD_EXTRA_EXPERIENCE_PER_UNIT_PERCENT
|Unknown
|-
!COMBAT_EXPERIENCE_IN_BORDERS_PERCENT
|Unknown
|-
!VICTORY_SOUNDTRACK_AVAILABLE
|Unknown
|-
!MAX_WITHDRAWAL_PROBABILITY
|Maximum chance a unit can withdraw
|-
!MAX_INTERCEPTION_PROBABILITY
|Maximum chance an air unit can intercept another
|-
!MAX_EVASION_PROBABILITY
|Maximum chance an air unit can evade interception
|-
!PLAYER_ALWAYS_RAZES_CITIES
|Unknown
|-
!MIN_WATER_SIZE_FOR_OCEAN
|Unknown
|-
!MIN_CITY_ATTACK_MODIFIER_FOR_SIEGE_TOWER
|Minimum city attach modifier needed for the siege tower to appear
|-
!ESPIONAGE_CITY_POP_EACH_MOD
|Percent cost change in espionage mission due to each population point
|-
!ESPIONAGE_CITY_TRADE_ROUTE_MOD
|Percent cost change in espionage mission due to each city trade route
|-
!ESPIONAGE_CITY_RELIGION_STATE_MOD
|Percent cost change in espionage mission due to each city religion
|-
!ESPIONAGE_CITY_HOLY_CITY_MOD
|Percent cost change in espionage mission due to holy city
|-
!ESPIONAGE_CULTURE_MULTIPLIER_MOD
|Unknown
|-
!ESPIONAGE_DISTANCE_MULTIPLIER_MOD
|Unknown
|-
!ESPIONAGE_SPENDING_MULTIPLIER
|Unknown
|-
!ESPIONAGE_EACH_TURN_UNIT_COST_DECREASE
|Unknown
|-
!ESPIONAGE_INTERCEPT_SPENDING_MAX
|Unknown
|-
!ESPIONAGE_INTERCEPT_COUNTERSPY
|Unknown
|-
!ESPIONAGE_INTERCEPT_COUNTERESPIONAGE_MISSION
|Unknown
|-
!ESPIONAGE_INTERCEPT_RECENT_MISSION
|Unknown
|-
!ESPIONAGE_SPY_REVEAL_IDENTITY_PERCENT
|Unknown
|-
!ESPIONAGE_SPY_INTERCEPT_MOD
|Unknown
|-
!ESPIONAGE_SPY_NO_INTRUDE_INTERCEPT_MOD
|Unknown
|-
!ESPIONAGE_SPY_MISSION_ESCAPE_MOD
|Unknown
|-
!FOW_WAS_VISIBLE_COLOR
|Unknown
|-
!FOW_MINIMAP_WAS_VISIBLE_COLOR
|Unknown
|-
!CITY_SCREEN_FOG_ENABLED
|Unknown
|-
!AI_CAN_DISBAND_UNITS
|Whether or not the AI can disband units
|-
!CAMERA_CITY_TURN
|Unknown
|-
!CAMERA_CITY_NO_PITCH
|Unknown
|-
!CAMERA_SPECIAL_PITCH
|Unknown
|-
!CITY_SCREEN_CLICK_WILL_EXIT
|Whether clicking outside the city radius will exit the city screen
|-
!WATER_POTENTIAL_CITY_WORK_FOR_AREA
|Unknown
|-
!LAND_UNITS_CAN_ATTACK_WATER_CITIES
|Whether or not land units can attack cities on located on water
|-
!CITY_MAX_NUM_BUILDINGS
|Unknown
|-
!RANGED_ATTACKS_USE_MOVES
|Number of moves used in a ranged attack
|-
!AI_SHOULDNT_MANAGE_PLOT_ASSIGNMENT
|Unknown
|-
!ROUTE_Z_BIAS
|Unknown
|-
!RIVER_Z_BIAS
|Unknown
|-
!ADVANCED_START_ALLOW_UNITS_OUTSIDE_CITIES
|Whether to allow units outside cities in advanced start
|-
!ADVANCED_START_MAX_UNITS_PER_CITY
|Maximum units per city in advanced start
|-
!ADVANCED_START_SIGHT_RANGE
|Starting sight range in advanced start
|-
!ADVANCED_START_CITY_COST
|Base city cost in advanced start
|-
!ADVANCED_START_CITY_COST_INCREASE
|Cost increase for cities in advanced start
|-
!ADVANCED_START_POPULATION_COST
|Base population cost in advanced start
|-
!ADVANCED_START_POPULATION_COST_INCREASE
|Cost increase for population in advanced start
|-
!ADVANCED_START_CULTURE_COST
|Base cost of culture in advanced start
|-
!ADVANCED_START_CULTURE_COST_INCREASE
|Cost increase in culture in advanced start
|-
!ADVANCED_START_VISIBILITY_COST
|Base cost of tile visibility in advanced start
|-
!ADVANCED_START_VISIBILITY_COST_INCREASE
|Cost increase of tile visibility in advanced start
|-
!ADVANCED_START_CITY_PLACEMENT_MAX_RANGE
|maximum range for city placement in advanced start
|-
!NEW_CITY_BUILDING_VALUE_MODIFIER
|Unknown
|-
!IGNORE_PLOT_GROUP_FOR_TRADE_ROUTES
|Unknown
|-
!EVENT_PROBABILITY_ROLL_SIDES
|Unknown
|-
!FIRST_EVENT_DELAY_TURNS
|Number of turns before first random event can happen
|-
!CIVILOPEDIA_SHOW_ACTIVE_CIVS_ONLY
|Whether the civilopedia can show civs not in the current game
|-
!USE_MODDERS_PLAYEROPTION_1
|Whether to show the additional player option left for modders
|-
!USE_MODDERS_PLAYEROPTION_2
|Whether to show the additional player option left for modders
|-
!USE_MODDERS_PLAYEROPTION_3
|Whether to show the additional player option left for modders
|-
!CITY_AIR_UNIT_CAPACITY
|Number of air units a city or fort can hold
|-
!COLONY_NUM_FREE_DEFENDERS
|Number of free units given to colonies
|-
!SHIP_BLOCKADE_RANGE
|Tile range that ships can blockade
|-
!PATH_DAMAGE_WEIGHT
|Unknown
|-
!USE_SPIES_NO_ENTER_BORDERS
|Whether or not spies can be blocked from entering borders
|-
!NO_ESPIONAGE_CULTURE_LEVEL_MODIFIER
|Percent change to culture level amounts when No Espionage is enabled
|-
!FORCE_UNOWNED_CITY_TIMER
|Unknown
|}

{{Civ4_XML_Files}}
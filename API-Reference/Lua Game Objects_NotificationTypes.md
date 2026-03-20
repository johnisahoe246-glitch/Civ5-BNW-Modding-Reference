Back to [[Lua Game Objects]]<br>
The NotificationTypes are defined somewhere in the DLL and are made available to Lua. They define the icon displayed (in conjunction with [[NotificationPanel.lua]]), sound played, and icon click behavior for the notifications. A notification can be triggered through Lua using the [[Lua_Game_Objects/Player#AddNotification|Player:AddNotification()]] method, and some NotificationTypes expect that function to supply either one or two extra integer parameters. 

=NotificationTypes=

==NOTIFICATION_GENERIC==
:Icon
::White exclamation point on blue background
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::None
:Extra Parameter 2
::None

==NOTIFICATION_TECH==
:Icon
::White exclamation point on blue background
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_FREE_TECH==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_POLICY==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_PRODUCTION==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_MET_MINOR==
:Icon
::White Capitol on blue/purple background
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_MINOR==
:Icon
::White Capitol on blue/purple background with overlaid small exclamation point on purple/red background
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_MINOR_QUEST==
:Icon
::White Capitol on blue/purple background with overlaid small exclamation point on purple/red background
:Sound
::No Description Available
:Left-Click
::Brings up minor civ diplomacy window with custom message
:Extra Parameter 1
::Player ID for the minor civ
:Extra Parameter 2
::No Description Available

==NOTIFICATION_ENEMY_IN_TERRITORY==
:Icon
::Unit icon fading into red targeting reticle
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Unit ID
:Extra Parameter 2
::No Description Available

==NOTIFICATION_CITY_RANGE_ATTACK==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_BARBARIAN==
:Icon
::Barbarian Camp icon; only appears to show if associated plot actually contains a camp.
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_GOODY==
:Icon
::Ancient Ruins icon; only appears to show if associated plot actually contains ruins.
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_BUY_TILE==
:Icon
::Spinning coin on pink hex
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_CITY_GROWTH==
:Icon
::Green citizen icon fading into "+1"
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_CITY_TILE==
:Icon
::Solid pink hex
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DEMAND_RESOURCE==
:Icon
::Resource Icon
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Resource ID
:Extra Parameter 2
::No Description Available

==NOTIFICATION_UNIT_PROMOTION==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_WONDER_COMPLETED_ACTIVE_PLAYER==
:Icon
::Wonder icon with optional overlaid small civ icon
:Sound
::No Description Available
:Left-Click
::Wonder popup
:Extra Parameter 1
::Building ID for wonder
:Extra Parameter 2
::Player ID; if this is -1, the overlaid civ icon does not appear

==NOTIFICATION_WONDER_COMPLETED==
:Icon
::Wonder icon with optional overlaid small civ icon
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Building ID for wonder
:Extra Parameter 2
::Player ID; if this is -1, the overlaid civ icon does not appear

==NOTIFICATION_WONDER_BEATEN==
:Icon
::Wonder icon with optional overlaid small civ icon
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Building ID for wonder
:Extra Parameter 2
::Player ID; if this is -1, the overlaid civ icon does not appear

==NOTIFICATION_GOLDEN_AGE_BEGUN_ACTIVE_PLAYER==
:Icon
::Yellow diamond on blue background
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_GOLDEN_AGE_ENDED_ACTIVE_PLAYER==
:Icon
::Yellow diamond on blue background
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_GREAT_PERSON_ACTIVE_PLAYER==
:Icon
::Unit icon
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Unit ID; can be any type of unit
:Extra Parameter 2
::No Description Available

==NOTIFICATION_STARVING==
:Icon
::Red Citizen Icon
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_WAR_ACTIVE_PLAYER==
:Icon
::Civ icon with crossed-swords
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Player ID; if -1 the civ icon is a question mark
:Extra Parameter 2
::No Description Available

==NOTIFICATION_WAR==
:Icon
::Crossed swords on yellow background with small civ icons overlaid on left and right
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Player ID for first civ (displayed on right); if -1 the civ icon is a question mark
:Extra Parameter 2
::Player ID for second civ (displayed on left); if -1 the civ icon is a question mark

==NOTIFICATION_PEACE_ACTIVE_PLAYER==
:Icon
::Civ icon with laurel branches
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Player ID; if -1 the civ icon is a question mark
:Extra Parameter 2
::No Description Available

==NOTIFICATION_PEACE==
:Icon
::Laurel branches on yellow background with small civ icons overlaid on top and bottom
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Player ID for first civ (displayed on bottom); if -1 the civ icon is a question mark
:Extra Parameter 2
::Player ID for second civ (displayed on top); if -1 the civ icon is a question mark


==NOTIFICATION_VICTORY==
:Icon
::Spinning trophy on yellow background
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_UNIT_DIED==
:Icon
::Unit icon with crossed swords
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Unit ID
:Extra Parameter 2
::No Description Available

==NOTIFICATION_CITY_LOST==
:Icon
::Capitol with red/yellow background
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_CAPITAL_LOST_ACTIVE_PLAYER==
:Icon
::Capitol with red/yellow background
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_CAPITAL_LOST==
:Icon
::Capitol with red/yellow background
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_CAPITAL_RECOVERED==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_PLAYER_KILLED==
:Icon
::Capitol with red/yellow background
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DISCOVERED_LUXURY_RESOURCE==
:Icon
::Resource icon with overlaid small happy face
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Resource ID; can be any type of resource
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DISCOVERED_STRATEGIC_RESOURCE==
:Icon
::Resource icon with overlaid small shield
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Resource ID; can be any type of resource
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DISCOVERED_BONUS_RESOURCE==
:Icon
::Resource icon with no overlay
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Resource ID; can be any type of resource
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DIPLO_VOTE==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_RELIGION_RACE==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_EXPLORATION_RACE==
:Icon
::Natural Wonder icon
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Feature ID; the icon for this feature is shown if this ID is for a natural wonder, but an icon which looks like [http://en.wikipedia.org/wiki/Delicate_Arch Delicate Arch] will be shown otherwise
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DIPLOMACY_DECLARATION==
:Icon
::Spinning yellow globe with laurel leaves
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DEAL_EXPIRED_GPT==
:Icon
::Spinning yellow globe with laurel leaves and a large red X
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DEAL_EXPIRED_RESOURCE==
:Icon
::Spinning yellow globe with laurel leaves and a large red X
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DEAL_EXPIRED_OPEN_BORDERS==
:Icon
::Spinning yellow globe with laurel leaves and a large red X
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DEAL_EXPIRED_DEFENSIVE_PACT==
:Icon
::Spinning yellow globe with laurel leaves and a large red X
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DEAL_EXPIRED_RESEARCH_AGREEMENT==
:Icon
::Spinning yellow globe with laurel leaves and a large red X
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DEAL_EXPIRED_TRADE_AGREEMENT==
:Icon
::Spinning yellow globe with laurel leaves and a large red X
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_TECH_AWARD==
:Icon
::Tech icon
:Sound
::No Description Available
:Left-Click
::Tech popup
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::Tech ID

==NOTIFICATION_PLAYER_DEAL==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_PLAYER_DEAL_RECEIVED==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_PLAYER_DEAL_RESOLVED==
:Icon
::Spinning globe with laurel leaves
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_PROJECT_COMPLETED==
:Icon
::Project icon with optional overlaid small civ icon
:Sound
::No Description Available
:Left-Click
::Zoom to plot
:Extra Parameter 1
::Project ID
:Extra Parameter 2
::Player ID; if this is -1, the overlaid civ icon does not appear

==NOTIFICATION_REBELS==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_FREE_POLICY==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_FREE_GREAT_PERSON==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_DENUNCIATION_EXPIRED==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available

==NOTIFICATION_FRIENDSHIP_EXPIRED==
:Icon
::No Description Available
:Sound
::No Description Available
:Left-Click
::No Description Available
:Extra Parameter 1
::No Description Available
:Extra Parameter 2
::No Description Available
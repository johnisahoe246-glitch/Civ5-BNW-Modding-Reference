==Description==
[http://wiki.2kgames.com/civ5/index.php/Lua_Game_Objects/Events Description] from the official wiki: 

===Summary===

This event is triggered when a [[Lua Game Objects/City|city]] is created.

===Listener reference===

listener( vHexPos, ePlayerID, iCityID, eArtStyleType, eEraType, iContinent, iPopulationSize, iSize, iFogState )

*'''vHexPos''' - Vector3 containing city x,y,z coordinates which can be converted to map coordinates with the ToGridFromHex function e.g. 
  local iX, iY = ToGridFromHex( vHexPos.x, vHexPos.y ) 
*'''ePlayerID''' - ID of the player who owns the created city; index into global Players table 
*'''iCityID''' - ID of the city that was created; note IDs are specific to player and not truly unique
*'''eArtStyleType''' - art style of city graphics; compare with types from ArtStyleTypes table (e.g. GameInfoTypes.ARTSTYLE_ASIAN) 
*'''eEraType''' - era of city graphics; compare with types from Eras table (e.g. GameInfoTypes.ERA_ANCIENT)
*'''iContinent''' - ID of continent where city is located 
*'''iPopulationSize''' - unknown; name based on reference in original game files (UnitFlagManager.lua and CityBannerManager.lua) 
*'''iSize''' - unknown; name based on reference in original game files (UnitFlagManager.lua and CityBannerManager.lua) 
*'''iFogState''' - visibility of this city for Active Player
::0 = tile completely hidden by FoW 
::1 = tile revealed but not currently in vision 
::2 = tile in vision
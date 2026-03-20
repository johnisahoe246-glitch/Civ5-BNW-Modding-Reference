=Overview=
MapView 2.10 and any version above will support Python scripting opportunities.
This article tries to give you a decent impression about the things that are possible throught this interface.
== Globals ==
=== mvMap ===
'''mvMap''' is always the map that is currently shown in the main screen. 
=== mvRules ===
'''mvRules''' is always the current ruleset of the selected mod. You can use it to find out about what the mod is supplying. 
== How to get a Tile? ==
This code will iterate over all fields from the currently shown map

 for x in range(0, mvMap.GetWidth()):
     for y in range(0, mvMap.GetHeight()):
         mvMap.Tile(x,y)

Simple Script printing the terrain type of all fields

 for x in range(0, mvMap.GetWidth()):
     for y in range(0, mvMap.GetHeight()):
         print mvMap.Tile(x,y).Terrain().Get()
== Classes ==
=== Map ===
 int GetWidth()
 int GetHeight()
 Tile Tile(int, int)
 void Refresh()
 Team AddTeam()
 Player AddPlayer()
=== Tile ===
 //getter
 Terrain Terrain()
 Bonus Bonus()
 Feature Feature()
 Route Route()
 Improvement Improvement()
 River River()
 City City()
 int GetUnitCount
 Unit GetUnit()
 //creators
 //other
 void DeleteAllUnits()
 void DeleteCity()
 void DeleteBonus()
 void DeleteFeature()
 void DeleteRiver()
 void DeleteRoute()
 void DeleteImprovement()
 bool IsNextToLand()
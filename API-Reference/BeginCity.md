'''BeginCity''' is the subsection that defines a city at this plot. A city is defined in the following way:
 BeginCity
  CityOwner=AAAA
  CityName=BBBB
  CityPopulation=CCCC
  ProductionUnit=DDDD
  ProductionBuilding=EEEE
  ProductionProject=FFFF
  ProductionProcess=GGGG
  BuildingType=HHHH
  ReligionType=IIII
  HolyCityReligionType=JJJJ
  ScriptData=KKKK
  PlayerLLLLCulture=MMMM
 EndCity
Where:
* AAAA = the city owner. Similar to unit owner it is the value between 0 and 17 of the player who owns this city.
* BBBB = the name of the city. This can be any value. EG: CityName=My City
* CCCC = the starting population in the city. This is how many population points the city starts with.
* DDDD = the unit that the city is building at game start. Only one Production type is used (the first one in the city definition). These values are defined in [[Civ4UnitInfos|CIV4UnitInfos.xml]]
* EEEE = the building that the city is building at game start. Only one Production type is used (the first one in the city definition). These values are defined in [[Civ4BuildingInfos|CIV4BuildingInfos.xml]]
* FFFF = the project that the city is building at game start. Only one Production type is used (the first one in the city definition). These values are defined in [[Civ4ProjectInfo|CIV4ProjectInfo.xml]]
* GGGG = the process (science/wealth/culture) that the city is building at game start. Only one Production type is used (the first one in the city definition). These values are defined in [[Civ4ProcessInfo|CIV4ProcessInfo.xml]]
* HHHH = the buildings that the city already has at game start. Any number of BuildingTypes can be defined on seperate lines. These values are defined in [[Civ4BuildingInfos|CIV4BuildingInfos.xml]]
* IIII = the religions that the city has at game start. Any number of religions can be defined on seperate lines. These values are defined in [[Civ4ReligionInfos|CIV4RelgionInfos.xml]]
* JJJJ = the Holy City of the defined religions. Any number of these can be defined on seperate lines. These values are defined in [[Civ4ReligionInfos|CIV4ReligionInfos.xml]]
* KKKK = any scripts assigned to the city. This analysis does not go into these scripts.
* LLLL & MMMM = the starting culture that the city has. LLLL is the player number and MMMM is the amount of culture. EG: Player3Culture=100 means this city begins with 100 points of player 3's culture. You can define a culture level for any number of players.
{{Civ4_World_Builder}}
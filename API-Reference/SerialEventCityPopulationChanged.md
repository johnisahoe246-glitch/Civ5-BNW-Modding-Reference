==Description==
Fired when a population of a particular [[Lua Game Objects/City|city]] was changed.

[http://wiki.2kgames.com/civ5/index.php/Lua_SerialEventCityPopulationChanged Description on the official wiki] is wrong: event is fired for both human player and AIs, for discovered and yet not discovered cities as well.
==Example==
  function OnCityPopulationChanged(x, y, newPop)
    local pPlot = [[Lua Game Objects/Map|Map]].[[GetPlot]]([[ToGridFromHex]](x, y))
    local pCity = pPlot:[[GetPlotCity()]]
    local pPlayer = [[Players]][pCity:[[GetOwner()]]]
    DoSomething(pCity)
  end
  Events.SerialEventCityPopulationChanged.Add(OnCityPopulationChanged)
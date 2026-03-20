==Description==
Sets the size of population in a subject city.

The second parameter should be ''true''. Otherwise, number of citizens would not be changed, whereas city size and corresponding food consumption etc would be increased.
==Example==
(from Emigration v.2 mod)
  function movePopulation(fromPlayer, fromCity, toPlayer)
    fromCity:'''''SetPopulation'''''(fromCity:GetPopulation() - 1, true);	--decrease population in a source city
    local toCity = getCityByIndex(toPlayer, Map.Rand(toPlayer:GetNumCities(), "Random city to emigrate to - Lua"));
    if toCity == nil then return end;
    toCity:'''''SetPopulation'''''(toCity:GetPopulation() + 1, true);	--increase population in a destination city
    <...>
  end

  function getCityByIndex(player, N)
    local n = 0;
    for city in player:Cities() do
      if (n == N) then
        return city;
      end
      n = n + 1;
    end
  end
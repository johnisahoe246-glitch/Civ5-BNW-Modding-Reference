Up: [[Lua Game Events]]

==Description==
Fired when [[Lua Game Objects/City|city]] is captured '''or traded to an another civ'''. 

==Example==
([http://forums.2kgames.com/showthread.php?113029-Reward-for-conquering-a-Civilization by whoward69])
  function OnCityCaptured(hexPos, playerID, cityID, newPlayerID)
    -- Empire destroyed?
    if (Players[playerID]:GetNumCities() == 0) then
      if (Game.GetActivePlayer() == newPlayerID) then
        -- Captured by player
        if (Players[playerID]:IsMinorCiv()) then
          -- It was a minor
        else
          -- It was a major
        end
      else
        -- Captured by AI
      end
    end
  end
  Events.SerialEventCityCaptured.Add(OnCityCaptured)

*hexPos argument passes encoded coordinates. Use it to get a corresponding plot:
  local pPlot = Map.GetPlot(ToGridFromHex(hexPos)
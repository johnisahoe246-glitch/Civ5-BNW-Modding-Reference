Up: [[Lua Game Events]]


==Description==
Fired when something in a particular [[Lua Game Objects/City|city]] was changed.
E.g. building created/sold, specialists reallocated, and some other things.

==Example==
(from SmoothCityBanner v.2 mod):

  function OnSpecificCityInfoDirty(iPlayerID, iCityID, eUpdateType)
      if (eUpdateType == [[Lua Game Objects/CityUpdateTypes|CityUpdateTypes]].CITY_UPDATE_TYPE_BANNER) then
          local playerTable = Instances[ iPlayerID ];
          if playerTable == nil then
              return;
          end
          local instance = playerTable[ iCityID ];
          if instance == nil then
              return;
          end
      RefreshCityBanner(instance);
      end
  end
  Events.SpecificCityInfoDirty.Add(OnSpecificCityInfoDirty);
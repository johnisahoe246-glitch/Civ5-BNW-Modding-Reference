==Description==
Fired when it is determined wherever a player can build a specific building or not.
Returning ''false'' from the listener function would make a building not buildable.
==Example==
([http://forums.civfanatics.com/showthread.php?t=449431 by Pazyryk])

Let's say you want a simple policy prerequisite to build a building (there isn't one in the base game).
You can add columns to existing core tables via SQL. Here's the code you need in an SQL file:
  ALTER TABLE Buildings ADD COLUMN 'PrereqPolicy' TEXT DEFAULT NULL;
SQL is added exactly as you add XML files (as an OnModActivated). Just make sure that the above file runs before your XML where you are using the new "PrereqPolicy" tag.
Now you need to add some Lua code to tell the dll what to do with this new table column:
  GameEvents.PlayerCanConstruct.Add(
  function(iPlayer, buildingTypeID)
    local prereqPolicy = GameInfo.Buildings[buildingTypeID].PrereqPolicy
    if prereqPolicy then
      local player = Players[iPlayer]
      local policyID = GameInfo.Policies[prereqPolicy].ID
      if not player:HasPolicy(policyID) then
        return false
      end
    end
    return true
  end)
That's it! You can now use this new tag to make any building construction dependent on having any particular policy, just like you use any other xml tag.


Following the example above, you should be able to add PolicyPrereq tags to Units and Techs in a similar way using these GameEvents:
  GameEvents.PlayerCanTrain.Add(function(iPlayer, unitTypeID) ... end)
  GameEvents.PlayerCanResearch.Add(function(iPlayer, techTypeID) ... end)

One suggestion: I actually add the above tag as "PrereqPolicy_paz". This is so that there are no problems down the road if the developers add a tag with this exact name (or perhaps a dll modder, once that is possible).

Also note that the above prereq will not be added to the pedia. You'll have to do that yourself. Otherwise, there will be no indication in the game why the building cannot be built.
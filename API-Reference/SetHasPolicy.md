==Description==
Sets player having a specified policy. Increases next policy cost. 
==Example==
([http://forums.civfanatics.com/showpost.php?p=11268848&postcount=12 by Androrc the Orc])
  function TheHumanGenomeProjectEffects( iPlayer )
  	local player = Players[iPlayer]
  	local team = Teams[player:GetTeam()]
  	local data = load( player, "TheHumanGenomeProjectApplied" ) or false
  
  	if (team:GetProjectCount(GameInfo.Projects["PROJECT_THE_HUMAN_GENOME_PROJECT"].ID) > 0 and not data) then
  		player:SetHasPolicy(GameInfo.Policies["POLICY_PROJECT_THE_HUMAN_GENOME_PROJECT"].ID, true)
  		save( player, "TheHumanGenomeProjectApplied", true )
  	end
  end
  
  GameEvents.PlayerDoTurn.Add( TheHumanGenomeProjectEffects )
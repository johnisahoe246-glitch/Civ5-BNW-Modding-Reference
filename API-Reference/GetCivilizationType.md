==Description==
Returns a civilization type value for a major civ player.
==Example==
(from Emigration v.2 mod)
  function GetPlayerName(player)	
  	if player:IsMinorCiv() then
  		local minorCivType = player:GetMinorCivType();
  		local minorCivInfo = GameInfo.MinorCivilizations[minorCivType];
  		return Locale.ConvertTextKey(minorCivInfo.Description);
  	end
  	local iCivType = player:GetCivilizationType();
  	local civInfo = GameInfo.Civilizations[iCivType];			
  	return Locale.ConvertTextKey(civInfo.Description);	
  end
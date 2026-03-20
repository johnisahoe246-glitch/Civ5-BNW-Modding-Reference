==Description==
Returns true if a player has a specified policy.
==Example==
  function hasPolicy(pPlayer, policyType)
  	for policy in GameInfo.Policies() do
  		if policy.Type == policyType then
  			return pPlayer:'''''HasPolicy'''''(policy.ID);
  		end
  	end
  	return false;
  end
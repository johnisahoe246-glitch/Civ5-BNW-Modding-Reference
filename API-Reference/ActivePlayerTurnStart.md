Up: [[Lua Game Events]]
==Description==
This event is fired on the start of the human [[Lua Game Objects/Player|player]]'s turn (not fired for AIs).
Can be used to do some per turn calculations.

==Example==
  function NewTurn()
    for _, pPlayer in pairs([[Players]]) do  --loop through all players
      UpdateSomething(pPlayer);
    end
  end
  Events.ActivePlayerTurnStart.Add( NewTurn );
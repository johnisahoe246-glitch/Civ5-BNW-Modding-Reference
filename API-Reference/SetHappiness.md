Up: [[Lua Game Objects/Player]]


From [http://forums.civfanatics.com/showthread.php?t=429585 conversation] on the civfanatics forum:
:''It's not even that it resets the next turn, it's actually resetting at the END of your turn, when the game does one final recalculation for all of the yields and such. So SetHappiness actually does nothing; while the UI will show a higher value for this turn, the value is reset BEFORE Happiness is used to increment Golden Ages or check for the effects of negative Happiness.''


Recommendations on how to mod happiness are also given in that thread.
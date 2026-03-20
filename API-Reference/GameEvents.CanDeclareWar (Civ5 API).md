{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Allows provision of criteria for the ability to declare war. As this is a TestAll event, all listeners must return '''true''' for the action to be permitted. As wars are between teams, it is based entirely on teams rather than players (as far as can be inferred from scenario files).


=Usage=
<code>'''bool''' GameEvents.CanDeclareWar<b>(</b>{{Type5|TeamID}} myTeam, {{Type5|TeamID}} theirTeam<b>)</b></code>


'''Event Type'''
:Unknown

'''Returned Value'''
:Return '''true''' if war declaration is to be permitted; '''false''' if it is not.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|myTeam:
|valign="top"| ''The team of the player who is hypothetically trying to declare war.''
|-
|valign="top" style="padding-right:6px;"|theirTeam:
|valign="top"| ''The team of them player they are hypothetically trying to declare war on.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0254}}<syntaxhighlight lang="lua">GameEvents.CanDeclareWar.Add(function(myTeam, theirTeam)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0256}}<syntaxhighlight lang="lua">local myPlayer = -1;</syntaxhighlight>
{{CodeLine5|0257}}<syntaxhighlight lang="lua">local theirPlayer = -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">for iLoopPlayer = 0, GameDefines.MAX_CIV_PLAYERS-1, 1 do</syntaxhighlight>
{{CodeLine5|0260}}<syntaxhighlight lang="lua">   local pLoopPlayer = Players[iLoopPlayer];</syntaxhighlight>
{{CodeLine5|0261}}<syntaxhighlight lang="lua">   if (pLoopPlayer:GetTeam() == myTeam) then</syntaxhighlight>
{{CodeLine5|0262}}<syntaxhighlight lang="lua">   myPlayer = iLoopPlayer;</syntaxhighlight>
{{CodeLine5|0263}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0264}}<syntaxhighlight lang="lua">   if (pLoopPlayer:GetTeam() == theirTeam) then</syntaxhighlight>
{{CodeLine5|0265}}<syntaxhighlight lang="lua">   theirPlayer = iLoopPlayer;</syntaxhighlight>
{{CodeLine5|0266}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0267}}<syntaxhighlight lang="lua">   if (myPlayer ~= -1 and theirPlayer ~= -1) then</syntaxhighlight>
{{CodeLine5|0268}}<syntaxhighlight lang="lua">   break;</syntaxhighlight>
{{CodeLine5|0269}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0270}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">   print(myPlayer);</syntaxhighlight>
{{CodeLine5|0273}}<syntaxhighlight lang="lua">   print(Players[myPlayer]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">   local myStartingPlot = (Players[myPlayer]) and Players[myPlayer]:GetStartingPlot() or nil;</syntaxhighlight>
{{CodeLine5|0276}}<syntaxhighlight lang="lua">   local theirStartingPlot = (Players[theirPlayer]) and Players[theirPlayer]:GetStartingPlot() or nil;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">   if(myStartingPlot == nil or theirStartingPlot == nil) then</syntaxhighlight>
{{CodeLine5|0279}}<syntaxhighlight lang="lua">   -- no war.</syntaxhighlight>
{{CodeLine5|0280}}<syntaxhighlight lang="lua">   return false;</syntaxhighlight>
{{CodeLine5|0281}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">   -- No restrictions on native civs as either declarers or declarees</syntaxhighlight>
{{CodeLine5|0284}}<syntaxhighlight lang="lua">   if (myStartingPlot:GetX() < 50) then</syntaxhighlight>
{{CodeLine5|0285}}<syntaxhighlight lang="lua">   return true;</syntaxhighlight>
{{CodeLine5|0286}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0287}}<syntaxhighlight lang="lua">   if (theirStartingPlot:GetX() < 50) then</syntaxhighlight>
{{CodeLine5|0288}}<syntaxhighlight lang="lua">   return true;</syntaxhighlight>
{{CodeLine5|0289}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">   -- This is European on European, so check if power declaring war has piracy</syntaxhighlight>
{{CodeLine5|0292}}<syntaxhighlight lang="lua">   pTeam = Teams[myTeam];</syntaxhighlight>
{{CodeLine5|0293}}<syntaxhighlight lang="lua">   iTech = GameInfoTypes["TECH_PIRACY"];</syntaxhighlight>
{{CodeLine5|0294}}<syntaxhighlight lang="lua">   if (pTeam:GetTeamTechs():HasTech(iTech)) then</syntaxhighlight>
{{CodeLine5|0295}}<syntaxhighlight lang="lua">   return true;</syntaxhighlight>
{{CodeLine5|0296}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0298}}<syntaxhighlight lang="lua">   return false;</syntaxhighlight>
{{CodeLine5|0299}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanDeclareWar]]
[[Category:Civ5 Diplomacy API|CanDeclareWar]]
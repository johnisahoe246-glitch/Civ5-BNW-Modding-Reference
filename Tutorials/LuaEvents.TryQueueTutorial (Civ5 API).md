{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.TryQueueTutorial<b>(</b>'''string''' tutorialID, '''bool''' highPriority<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.TryQueueTutorial.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.TryQueueTutorial(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tutorialID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|highPriority:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1673}}<syntaxhighlight lang="lua">LuaEvents.TryQueueTutorial("CITY_SCREEN", true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0492}}<syntaxhighlight lang="lua">LuaEvents.TryQueueTutorial("DIPLO_TRADE_SCREEN", true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0659}}<syntaxhighlight lang="lua">LuaEvents.TryQueueTutorial.Add(function(tutorialID, highPriority)</syntaxhighlight>
{{CodeLine5|0660}}<syntaxhighlight lang="lua">--print("Trying to queue a tutorial");</syntaxhighlight>
{{CodeLine5|0661}}<syntaxhighlight lang="lua">for i,v in ipairs(TutorialInfo) do</syntaxhighlight>
{{CodeLine5|0662}}<syntaxhighlight lang="lua">   if(v.ID == tutorialID) then</syntaxhighlight>
{{CodeLine5|0663}}<syntaxhighlight lang="lua">   if(CanQueueTutorial(v)) then</syntaxhighlight>
{{CodeLine5|0664}}<syntaxhighlight lang="lua">   if(highPriority ~= nil) then</syntaxhighlight>
{{CodeLine5|0665}}<syntaxhighlight lang="lua">   QueueTutorial(v);</syntaxhighlight>
{{CodeLine5|0666}}<syntaxhighlight lang="lua">   ProcessActiveTutorialQueue();</syntaxhighlight>
{{CodeLine5|0667}}<syntaxhighlight lang="lua">   else</syntaxhighlight>
{{CodeLine5|0668}}<syntaxhighlight lang="lua">   local bWasEmpty = #g_ActiveTutorialQueue == 0;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0670}}<syntaxhighlight lang="lua">   QueueTutorial(v);</syntaxhighlight>
{{CodeLine5|0671}}<syntaxhighlight lang="lua">   if(bWasEmpty) then</syntaxhighlight>
{{CodeLine5|0672}}<syntaxhighlight lang="lua">   ProcessActiveTutorialQueue();</syntaxhighlight>
{{CodeLine5|0673}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0674}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0675}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0676}}<syntaxhighlight lang="lua">   break;</syntaxhighlight>
{{CodeLine5|0677}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0678}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0679}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TryQueueTutorial]]
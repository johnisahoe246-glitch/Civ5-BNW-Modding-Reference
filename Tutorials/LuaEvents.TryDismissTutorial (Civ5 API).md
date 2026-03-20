{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.TryDismissTutorial<b>(</b>'''string''' tutorialID<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.TryDismissTutorial.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.TryDismissTutorial(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tutorialID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">LuaEvents.TryDismissTutorial("CITY_SCREEN");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0497}}<syntaxhighlight lang="lua">LuaEvents.TryDismissTutorial("DIPLO_TRADE_SCREEN");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0681}}<syntaxhighlight lang="lua">LuaEvents.TryDismissTutorial.Add(function(tutorialID)</syntaxhighlight>
{{CodeLine5|0682}}<syntaxhighlight lang="lua">--print("Trying to dismiss a tutorial");</syntaxhighlight>
{{CodeLine5|0683}}<syntaxhighlight lang="lua">for i,v in ipairs(TutorialInfo) do</syntaxhighlight>
{{CodeLine5|0684}}<syntaxhighlight lang="lua">   if(v.ID == tutorialID) then</syntaxhighlight>
{{CodeLine5|0685}}<syntaxhighlight lang="lua">   DismissActiveTutorial(tutorial);</syntaxhighlight>
{{CodeLine5|0686}}<syntaxhighlight lang="lua">   break;</syntaxhighlight>
{{CodeLine5|0687}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0688}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0689}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TryDismissTutorial]]
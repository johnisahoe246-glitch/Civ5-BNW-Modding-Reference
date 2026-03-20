{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' Modding.GetEvaluatedFilePath<b>(</b>'''string''' myModId, '''unknown''' myModVersion, '''string''' customImage<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|myModId:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|myModVersion:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|customImage:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2315}}<syntaxhighlight lang="lua">local addinFile = Modding.GetEvaluatedFilePath(addin.ModID, addin.Version, addin.File);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">local customSetupFile = Modding.GetEvaluatedFilePath(entry.ModID, entry.Version, entry.File);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">local customImageFile = Modding.GetEvaluatedFilePath(customMod.ModID, customMod.Version, customImage);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">local scenarioMap = Modding.GetEvaluatedFilePath(myModId, myModVersion, "FoRScenario.Civ5Map");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">local randomMap = Modding.GetEvaluatedFilePath(MOD_ID, myModVersion, "Europe_Scenario.lua");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">local historicalMap = Modding.GetEvaluatedFilePath(MOD_ID, myModVersion, "MedievalWorld.Civ5Map");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MongolScenarioLoadScreen.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/MongolScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">local file = Modding.GetEvaluatedFilePath(myModId, myModVersion, "MongolScenario.Civ5Map");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ScenariosMenu.lua}}
:<code>UI/FrontEnd/ScenariosMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">local foregroundImageFile = Modding.GetEvaluatedFilePath(customMod.ModID, customMod.Version, customImage);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetEvaluatedFilePath]]
[[Category:Civ5 Movement API|GetEvaluatedFilePath]]
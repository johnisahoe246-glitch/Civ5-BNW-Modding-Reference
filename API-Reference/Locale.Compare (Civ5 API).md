{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Locale.Compare<b>(</b>'''string''' a, '''string''' b<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|a:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|b:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0411}}<syntaxhighlight lang="lua">table.sort(civs, function(a,b) return Locale.Compare(a.LeaderDescription, b.LeaderDescription) == -1; end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">table.sort(availablePantheonBeliefs, function(a,b) return Locale.Compare(a.Name, b.Name) < 0; end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0124}}<syntaxhighlight lang="lua">table.sort(availableFounderBeliefs, function(a,b) return Locale.Compare(a.Name, b.Name) < 0; end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">table.sort(availableFollowerBeliefs, function(a,b) return Locale.Compare(a.Name, b.Name) < 0; end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">table.sort(availableEnhancerBeliefs, function(a,b) return Locale.Compare(a.Name, b.Name) < 0; end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">table.sort(availableBonusBeliefs, function(a,b) return Locale.Compare(a.Name, b.Name) < 0; end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">return Locale.Compare(a.entryName, b.entryName) == -1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">return (Locale.Compare(a.text, b.text) == -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1509}}<syntaxhighlight lang="lua">return Locale.Compare(a[field], b[field]) == -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1513}}<syntaxhighlight lang="lua">return Locale.Compare(a[field], b[field]) == 1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0450}}<syntaxhighlight lang="lua">table.sort(sortedActivatedMods, function(a,b) return Locale.Compare(a.Title, b.Title) == -1 end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">return (Locale.Compare(a.DisplayName, b.DisplayName) == -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0048}}<syntaxhighlight lang="lua">return (Locale.Compare(a.DisplayName, b.DisplayName) == 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0635}}<syntaxhighlight lang="lua">return Locale.Compare(oa.Title, ob.Title) == -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">return Locale.Compare(ob.Title, oa.Title) == -1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0472}}<syntaxhighlight lang="lua">compareResult = Locale.Compare(aRowData[v.Column], bRowData[v.Column]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0475}}<syntaxhighlight lang="lua">compareResult = Locale.Compare(bRowData[v.Column], aRowData[v.Column]);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PremiumContentMenu.lua}}
:<code>UI/FrontEnd/PremiumContentMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">return Locale.Compare(a.Description, b.Description) == -1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0313}}<syntaxhighlight lang="lua">table.sort(sortedGreatPeople, function(a,b) return Locale.Compare(a,b) == -1 end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1223}}<syntaxhighlight lang="lua">table.sort(graphEntries, function(a,b) return Locale.Compare(a[1], b[1]) == -1; end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ScenariosMenu.lua}}
:<code>UI/FrontEnd/ScenariosMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">table.sort(g_ScenarioList, function(a,b) return Locale.Compare(a.DisplayName, b.DisplayName) == -1 end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">table.sort(civEntries, function(a, b) return Locale.Compare(a[1], b[1]) == -1 end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1036}}<syntaxhighlight lang="lua">table.sort(civEntries, function(a,b) return Locale.Compare(a.Title, b.Title) == -1; end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechButtonInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechTree/TechButtonInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">table.sort(sortedYieldChanges, function(a,b) return Locale.Compare(a[1], b[1]) == -1 end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">table.sort(v[2], function(a,b) return Locale.Compare(a,b) == -1 end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Compare]]
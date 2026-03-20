{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|City}} UI.GetHeadSelectedCity<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">local pCity = UI.GetHeadSelectedCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">if UI.GetHeadSelectedCity() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">Data1 = UI.GetHeadSelectedCity():GetID(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1693}}<syntaxhighlight lang="lua">local pHeadSelectedCity = UI.GetHeadSelectedCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1893}}<syntaxhighlight lang="lua">local city = UI.GetHeadSelectedCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1975}}<syntaxhighlight lang="lua">if (not UI.GetHeadSelectedCity():IsNoAutoAssignSpecialists()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1792}}<syntaxhighlight lang="lua">local pHeadCity = UI.GetHeadSelectedCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0290}}<syntaxhighlight lang="lua">lastCityEntered = UI.GetHeadSelectedCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">city = UI.GetHeadSelectedCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">local selectedCity = UI.GetHeadSelectedCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">if (UI.GetHeadSelectedCity() ~= nil) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHeadSelectedCity]]
[[Category:Civ5 Cities API|GetHeadSelectedCity]]
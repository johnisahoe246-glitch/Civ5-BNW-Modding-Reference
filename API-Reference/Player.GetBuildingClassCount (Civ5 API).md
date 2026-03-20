{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetBuildingClassCount<b>(</b>{{Type5|BuildingClassType}} buildingClass<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|buildingClass:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0808}}<syntaxhighlight lang="lua">elseif (pPlayer:GetBuildingClassCount(thisBuildingClass.ID) > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">if (Players[iPlayer]:GetBuildingClassCount(t.BuildingClass) > 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildingClassCount]]
[[Category:Civ5 Buildings API|GetBuildingClassCount]]
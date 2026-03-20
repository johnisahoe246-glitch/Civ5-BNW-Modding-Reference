{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:CanConstruct<b>(</b>{{Type5|BuildingType}} building, '''int''' continue, '''int''' testVisible, '''bool''' ignoreCost<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|continue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|testVisible:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ignoreCost:
|valign="top"| ''No description available.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
pCity:CanConstruct(100, 1, 1, 1));</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0359}}<syntaxhighlight lang="lua">if city:CanConstruct( buildingID, 0, 1 ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">if not city:CanConstruct( buildingID ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2909}}<syntaxhighlight lang="lua">if (pCity:CanConstruct(buildingID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2957}}<syntaxhighlight lang="lua">if (not pCity:CanConstruct(buildingID) and not pCity:IsHasBuilding(buildingID) and pCity:GetProductionBuilding() ~= buildingID) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanConstruct]]
[[Category:Civ5 City Production API|CanConstruct]]
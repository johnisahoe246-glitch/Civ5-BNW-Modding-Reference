{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetMinorCivType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">controls.StatusIcon:SetTexture( GameInfo.MinorCivTraits[ GameInfo.MinorCivilizations[ player:GetMinorCivType() ].MinorCivTrait ].TraitIcon );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0434}}<syntaxhighlight lang="lua">local minorCivType = pOtherPlayer:GetMinorCivType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0473}}<syntaxhighlight lang="lua">local sMinorCivType = pOtherPlayer:GetMinorCivType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0479}}<syntaxhighlight lang="lua">local sMinorCivType = pPlayer:GetMinorCivType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1309}}<syntaxhighlight lang="lua">local minorCivType = minorCivPlayer:GetMinorCivType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0810}}<syntaxhighlight lang="lua">local minorType = pPlayer:GetMinorCivType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1143}}<syntaxhighlight lang="lua">if (pPlayer:GetMinorCivType() == GameInfoTypes["MINOR_CIV_WITTENBERG"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1146}}<syntaxhighlight lang="lua">elseif (pPlayer:GetMinorCivType() == GameInfoTypes["MINOR_CIV_ZURICH"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1149}}<syntaxhighlight lang="lua">elseif (pPlayer:GetMinorCivType() == GameInfoTypes["MINOR_CIV_GENEVA"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1152}}<syntaxhighlight lang="lua">elseif (pPlayer:GetMinorCivType() == GameInfoTypes["MINOR_CIV_VATICAN_CITY"]) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMinorCivType]]
[[Category:Civ5 City States API|GetMinorCivType]]
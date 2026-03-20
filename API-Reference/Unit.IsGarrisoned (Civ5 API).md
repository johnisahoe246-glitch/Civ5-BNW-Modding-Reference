{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsGarrisoned<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1165}}<syntaxhighlight lang="lua">if unit ~= nil and cityBanners ~= nil and unit:IsGarrisoned() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">elseif( unit:IsGarrisoned()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">o.m_IsGarrisoned = pUnit:IsGarrisoned();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0492}}<syntaxhighlight lang="lua">if self.m_IsGarrisoned and not pUnit:IsGarrisoned() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0506}}<syntaxhighlight lang="lua">elseif( pUnit:IsGarrisoned() )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0596}}<syntaxhighlight lang="lua">if( test ~= nil and test:GetID() ~= self.m_UnitID and not test:IsGarrisoned() )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0848}}<syntaxhighlight lang="lua">if pUnit:IsGarrisoned() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0980}}<syntaxhighlight lang="lua">flag:GarrisonComplete( thisUnit:IsGarrisoned() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">if( test ~= nil and test:GetID() ~= self.m_UnitID and not test:IsGarrisoned() and not test:IsDead() and not test:IsDelayedDeath() )</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsGarrisoned]]
[[Category:Civ5 Units API|IsGarrisoned]]
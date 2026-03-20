{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} City:GetOriginalOwner<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0150}}<syntaxhighlight lang="lua">local isCapital = city:IsCapital() or Players[city:GetOriginalOwner()]:IsMinorCiv();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0424}}<syntaxhighlight lang="lua">local pOriginalOwner = Players[ city:GetOriginalOwner() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">if (pCity:GetOriginalOwner() ~= iEngland) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">local iOriginalOwner = pCity:GetOriginalOwner();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetOriginalOwner]]
[[Category:Civ5 Terrain Ownership API|GetOriginalOwner]]
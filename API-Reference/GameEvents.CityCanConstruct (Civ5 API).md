{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Similar to CanDeclareWar, this allows provision of critera for the ability to construct a particular building (including Wonders, presumably) in a particular city. Based on the behaviour in the 1066 scenario, it seems that returns of false lead to the building not appearing in the list of buildings available to construct, rather than being greyed out, but this hasn't been specifically checked. It makes some sense, though, as there's no way to provide a tooltip to explain the greying out under this mechanism.
As with CanDeclareWar, it's unclear whether multiple listeners' returns are combined with AND or OR; either seems possible according to the detailed explanation of how these events are handled.


=Usage=
<code>'''void''' GameEvents.CityCanConstruct<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|BuildingType}} buildingType<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''the index identifying the player who might or might not be able to construct''
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''the index identifying the city that might or might not be able to construct''
|-
|valign="top" style="padding-right:6px;"|buildingType:
|valign="top"| ''the ID of the building that might or might not be able to be constructed''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">GameEvents.CityCanConstruct.Add(function(iPlayer, iCity, iBuildingType)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">local iEngland = -1;</syntaxhighlight>
{{CodeLine5|0083}}<syntaxhighlight lang="lua">local iLondonX = 43;</syntaxhighlight>
{{CodeLine5|0084}}<syntaxhighlight lang="lua">local iLondonY = 17;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">for iPlayer = 0, 3, 1 do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">   local pPlayer = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0089}}<syntaxhighlight lang="lua">   local playerStartPlot = pPlayer:GetStartingPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">   -- London?</syntaxhighlight>
{{CodeLine5|0092}}<syntaxhighlight lang="lua">   if (playerStartPlot:GetX() == iLondonX and playerStartPlot:GetY() == iLondonY) then</syntaxhighlight>
{{CodeLine5|0093}}<syntaxhighlight lang="lua">   iEngland = iPlayer;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">   break;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0099}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0100}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">   local pPlayer = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0103}}<syntaxhighlight lang="lua">   local pCity = pPlayer:GetCityByID(iCity);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">   -- Shire Courts</syntaxhighlight>
{{CodeLine5|0106}}<syntaxhighlight lang="lua">   if (iBuildingType == GameInfo.Buildings["BUILDING_COURTHOUSE"].ID) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">   -- Only 8+ tiles from London</syntaxhighlight>
{{CodeLine5|0109}}<syntaxhighlight lang="lua">   if (Map.PlotDistance(pCity:GetX(), pCity:GetY(), iLondonX, iLondonY) < 8) then</syntaxhighlight>
{{CodeLine5|0110}}<syntaxhighlight lang="lua">   return false;</syntaxhighlight>
{{CodeLine5|0111}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">   -- Only in originally Anglo-Saxon cities</syntaxhighlight>
{{CodeLine5|0114}}<syntaxhighlight lang="lua">   if (pCity:GetOriginalOwner() ~= iEngland) then</syntaxhighlight>
{{CodeLine5|0115}}<syntaxhighlight lang="lua">   return false;</syntaxhighlight>
{{CodeLine5|0116}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0118}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">   -- Domesday Book (only in London)</syntaxhighlight>
{{CodeLine5|0121}}<syntaxhighlight lang="lua">   if (iBuildingType == GameInfo.Buildings["BUILDING_NATIONAL_COLLEGE"].ID) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">   if (pCity:GetX() ~= iLondonX or pCity:GetY() ~= iLondonY) then</syntaxhighlight>
{{CodeLine5|0124}}<syntaxhighlight lang="lua">   return false;</syntaxhighlight>
{{CodeLine5|0125}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">   return true;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CityCanConstruct]]
[[Category:Civ5 Cities API|CityCanConstruct]]
[[Category:Civ5 City Production API|CityCanConstruct]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetHappinessPerGarrisonedUnit<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0331}}<syntaxhighlight lang="lua">if (pPlayer:GetHappinessPerGarrisonedUnit() ~= 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">strGarrison = pPlayer:GetHappinessPerGarrisonedUnit();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">if( pPlayer:GetHappinessPerGarrisonedUnit() > 0 ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHappinessPerGarrisonedUnit]]
[[Category:Civ5 Happiness API|GetHappinessPerGarrisonedUnit]]
[[Category:Civ5 Units API|GetHappinessPerGarrisonedUnit]]
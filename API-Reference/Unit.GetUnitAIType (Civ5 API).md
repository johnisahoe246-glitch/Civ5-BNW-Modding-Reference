{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|UnitAIType}} Unit:GetUnitAIType<b>(</b><b>)</b></code>


'''Returned Value'''
:{{Type5|UnitAITypes}} ID


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0535}}<syntaxhighlight lang="lua">if (pUnit:GetUnitAIType() == GameInfo.UnitAIInfos.UNITAI_EXPLORE_SEA.ID) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnitAIType]]
[[Category:Civ5 Units API|GetUnitAIType]]
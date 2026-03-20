{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.ScenarioUnitTiersChanged<b>(</b>table('''string''' => {{Type5|PlayerID}}) tUnitTiers<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.ScenarioUnitTiersChanged.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.ScenarioUnitTiersChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tUnitTiers:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">LuaEvents.ScenarioUnitTiersChanged(tCopy);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0569}}<syntaxhighlight lang="lua">LuaEvents.ScenarioUnitTiersChanged.Add( ReceiveUnitTiersChanged );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0798}}<syntaxhighlight lang="lua">LuaEvents.ScenarioUnitTiersChanged(tUnitTiersCopy);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ScenarioUnitTiersChanged]]
[[Category:Civ5 Units API|ScenarioUnitTiersChanged]]
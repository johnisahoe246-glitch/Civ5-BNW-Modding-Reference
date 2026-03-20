{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventGameDataDirty<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventGameDataDirty.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventGameDataDirty(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">Events.SerialEventGameDataDirty.Add(OnGameDataDirty);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">Events.SerialEventGameDataDirty.Add(DoUpdateUNCountdown);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">Events.SerialEventGameDataDirty.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0796}}<syntaxhighlight lang="lua">Events.SerialEventGameDataDirty.Add( OnDirty );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">Events.SerialEventGameDataDirty.Add(OnTechPanelUpdated);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0119}}<syntaxhighlight lang="lua">Events.SerialEventGameDataDirty.Add( OnTechPanelUpdated );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0925}}<syntaxhighlight lang="lua">Events.SerialEventGameDataDirty.Add(OnTopPanelDirty);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventGameDataDirty]]
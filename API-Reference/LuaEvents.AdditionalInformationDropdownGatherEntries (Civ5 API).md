{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.AdditionalInformationDropdownGatherEntries<b>(</b>table('''int''' => '''table''') additionalEntries<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.AdditionalInformationDropdownGatherEntries.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.AdditionalInformationDropdownGatherEntries(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|additionalEntries:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">LuaEvents.AdditionalInformationDropdownGatherEntries(additionalEntries);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1687}}<syntaxhighlight lang="lua">LuaEvents.AdditionalInformationDropdownGatherEntries.Add(function(entries)</syntaxhighlight>
{{CodeLine5|1688}}<syntaxhighlight lang="lua">if (not Game.IsOption("GAMEOPTION_NO_ESPIONAGE")) then</syntaxhighlight>
{{CodeLine5|1689}}<syntaxhighlight lang="lua">table.insert(entries, {</syntaxhighlight>
{{CodeLine5|1690}}<syntaxhighlight lang="lua">text = Locale.Lookup("TXT_KEY_EO_TITLE"),</syntaxhighlight>
{{CodeLine5|1691}}<syntaxhighlight lang="lua">call = function()</syntaxhighlight>
{{CodeLine5|1692}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup{</syntaxhighlight>
{{CodeLine5|1693}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_ESPIONAGE_OVERVIEW,</syntaxhighlight>
{{CodeLine5|1694}}<syntaxhighlight lang="lua">};</syntaxhighlight>
{{CodeLine5|1695}}<syntaxhighlight lang="lua">end,</syntaxhighlight>
{{CodeLine5|1696}}<syntaxhighlight lang="lua">});</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1698}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|1699}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0804}}<syntaxhighlight lang="lua">LuaEvents.AdditionalInformationDropdownGatherEntries.Add(function(entries)</syntaxhighlight>
{{CodeLine5|0805}}<syntaxhighlight lang="lua">table.insert(entries, {</syntaxhighlight>
{{CodeLine5|0806}}<syntaxhighlight lang="lua">text=Locale.Lookup("TXT_KEY_RELIGION_OVERVIEW"),</syntaxhighlight>
{{CodeLine5|0807}}<syntaxhighlight lang="lua">call=function()</syntaxhighlight>
{{CodeLine5|0808}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup{</syntaxhighlight>
{{CodeLine5|0809}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_RELIGION_OVERVIEW,</syntaxhighlight>
{{CodeLine5|0810}}<syntaxhighlight lang="lua">};</syntaxhighlight>
{{CodeLine5|0811}}<syntaxhighlight lang="lua">end,</syntaxhighlight>
{{CodeLine5|0812}}<syntaxhighlight lang="lua">});</syntaxhighlight>
{{CodeLine5|0813}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AdditionalInformationDropdownGatherEntries]]
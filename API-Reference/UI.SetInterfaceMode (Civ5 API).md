{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.SetInterfaceMode<b>(</b>{{Type5|InterfaceMode}} interfaceModeSelection<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|interfaceModeSelection:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1002}}<syntaxhighlight lang="lua">UI.SetInterfaceMode(InterfaceModeTypes.INTERFACEMODE_CITY_RANGE_ATTACK);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1068}}<syntaxhighlight lang="lua">UI.SetInterfaceMode(InterfaceModeTypes.INTERFACEMODE_PLACE_UNIT);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityPlotManagementPopup.lua}}
:<code>UI/InGame/PopupsGeneric/CityPlotManagementPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">UI.SetInterfaceMode(InterfaceModeTypes.INTERFACEMODE_CITY_PLOT_SELECTION);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0574}}<syntaxhighlight lang="lua">UI.SetInterfaceMode(interfaceModeSelection);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">UI.SetInterfaceMode(InterfaceModeTypes.INTERFACEMODE_SELECTION);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2116}}<syntaxhighlight lang="lua">UI.SetInterfaceMode(InterfaceModeTypes.INTERFACEMODE_PURCHASE_PLOT);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetInterfaceMode]]
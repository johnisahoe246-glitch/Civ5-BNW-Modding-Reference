{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.BuildingLibrarySwap<b>(</b>'''int''' assetCulture, '''int''' assetEra<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.BuildingLibrarySwap.Add(''<function handler>'')</code> or invoke it directly through <code>Events.BuildingLibrarySwap(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|assetCulture:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|assetEra:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0393}}<syntaxhighlight lang="lua">Events.BuildingLibrarySwap( g_iAssetCulture, g_iAssetEra );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|BuildingLibrarySwap]]
[[Category:Civ5 Buildings API|BuildingLibrarySwap]]
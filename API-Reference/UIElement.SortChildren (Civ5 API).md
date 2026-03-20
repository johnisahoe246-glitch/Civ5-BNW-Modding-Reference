{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SortChildren<b>(</b>('''void''' func<b>(</b>'''unknown''' a, '''unknown''' b<b>)</b>) SortFunction<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|SortFunction:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0268}}<syntaxhighlight lang="lua">Controls.MainStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1251}}<syntaxhighlight lang="lua">Controls.BuildingStack:SortChildren( CVSortFunction );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4663}}<syntaxhighlight lang="lua">Controls.ListOfArticles:SortChildren( SortFunction );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">Controls.ArtistStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeLine5|0168}}<syntaxhighlight lang="lua">Controls.EngineerStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeLine5|0169}}<syntaxhighlight lang="lua">Controls.MerchantStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeLine5|0170}}<syntaxhighlight lang="lua">Controls.ScientistStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0566}}<syntaxhighlight lang="lua">Controls.LoadFileButtonStack:SortChildren( CloudSaveSort );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0587}}<syntaxhighlight lang="lua">Controls.LoadFileButtonStack:SortChildren( g_CurrentSort );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0742}}<syntaxhighlight lang="lua">Controls.LoadFileButtonStack:SortChildren( v[2] );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0487}}<syntaxhighlight lang="lua">Controls.ListingStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0347}}<syntaxhighlight lang="lua">Controls.MilitaryStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeLine5|0348}}<syntaxhighlight lang="lua">Controls.CivilianStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">teamEntry.TeamStack:SortChildren( MPListSort );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0300}}<syntaxhighlight lang="lua">Controls.MPListStack:SortChildren( MPListSort );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">Controls.LuxuryStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeLine5|0146}}<syntaxhighlight lang="lua">Controls.StrategicStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeLine5|0147}}<syntaxhighlight lang="lua">Controls.BonusStack:SortChildren( SortFunction );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SortChildren]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:BuildInstanceForControl<b>(</b>'''string''' arg0, '''table''' arg1, {{Type5|Stack}} arg2<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1332}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "PlayerSlot", g_SlotInstances[i], Controls.SlotStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ItemInstance", controlTable, stackControl );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0103}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "CityInstance", instance, Controls.MainStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "Entry", instance, Controls.MainStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ChatEntry", controlTable, Controls.ChatStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "DealButtonInstance", controlTable, Controls.CurrentDealsStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "DealButtonInstance", controlTable, Controls.HistoricDealsStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl("MajorInstance", controlTable, Controls.ItemStack);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl("LTextEntry", textControls, controlTable.PoliciesStack);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl("LTextEntry", textControls, controlTable.WondersStack);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl("TextEntry", textControls, controlTable.PactStack);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.CityStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0254}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.TradeStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.BuildingsStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ItemInstance", controlTable, Controls.DifficultyStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "SelectCivInstance", controlTable, Controls.SelectCivStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "NaturalWonder", instance, Controls.NaturalWonderStore );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "SettlerReccomendation", instance, Controls.SettlerReccomendationStore );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "WorkerReccomendation", instance, Controls.WorkerReccomendationStore );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.LuxuryHappinessStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.CityBuildingStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0311}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.TradeRouteStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.GarrisonStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0566}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.CityUnhappinessStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0623}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ResourceEntry", instance, Controls.ResourcesAvailableStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0666}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ResourceEntry", instance, Controls.ResourcesImportedStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0708}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ResourceEntry", instance, Controls.ResourcesExportedStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0749}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ResourceEntry", instance, Controls.ResourcesLocalStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TradeEntry", instance, Controls.LocalCityStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstanceManager.lua}}
:<code>UI/InstanceManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl(self.m_InstanceName, controlTable, self.m_ParentControl);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "PlayerEntry", controlTable, Controls.MPListStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TeamEntry", teamEntry, Controls.MPListStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0232}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "PlayerEntry", controlTable, teamEntry.TeamStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0177}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( name .. "Item", instance, Controls.SmallStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "ItemInstance", controlTable, Controls.Stack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1269}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "PlayerSlot", instance, Controls.SlotStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2252}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "PocketResource", controlTable, stack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2268}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TableStrategic", controlTable, stack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2292}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "TableLuxury", controlTable, stack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2782}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "OtherPlayerEntry", controlTable, Controls.UsPocketLeaderStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2792}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "OtherPlayerEntry", controlTable, Controls.ThemPocketLeaderStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2802}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "OtherPlayerEntry", controlTable, Controls.UsTableMakePeaceStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2812}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "OtherPlayerEntry", controlTable, Controls.UsTableDeclareWarStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2822}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "OtherPlayerEntry", controlTable, Controls.ThemTableMakePeaceStack );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2832}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "OtherPlayerEntry", controlTable, Controls.ThemTableDeclareWarStack );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "AirButton", o.m_CargoControls, o.m_Instance.AirAnchor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1037}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl( "CityFlag", cityFlagInstance, Controls.CityContainer );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">ContextPtr:BuildInstanceForControl("TokenInstance", t, cStack);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|BuildInstanceForControl]]
[[Category:Civ5 Improvements API|BuildInstanceForControl]]
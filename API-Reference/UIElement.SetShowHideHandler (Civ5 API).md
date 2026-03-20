{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetShowHideHandler<b>(</b>('''void''' func<b>(</b>'''bool''' isHide, '''int''' bInitState<b>)</b>) ShowHide<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ShowHide:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 139 are listed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0460}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler( ShowHide );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1287}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler( ShowHideHandler );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler(ShowHideHandler);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EULA.lua}}
:<code>UI/FrontEnd/Modding/EULA.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler(function(isHide)</syntaxhighlight>
{{CodeLine5|0038}}<syntaxhighlight lang="lua">--UNCOMMENT THIS BLOCK IF YOU WISH TO ONLY</syntaxhighlight>
{{CodeLine5|0039}}<syntaxhighlight lang="lua">--SHOW THE EULA ONCE PER APPLICATION RUN</syntaxhighlight>
{{CodeLine5|0040}}<syntaxhighlight lang="lua">--if not isHide and g_HasAcceptedEULA then</syntaxhighlight>
{{CodeLine5|0041}}<syntaxhighlight lang="lua">--   NavigateForward();</syntaxhighlight>
{{CodeLine5|0042}}<syntaxhighlight lang="lua">--end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0044}}<syntaxhighlight lang="lua">--if(not isHide and g_QueueEulaToHide) then</syntaxhighlight>
{{CodeLine5|0045}}<syntaxhighlight lang="lua">--   NavigateBack();</syntaxhighlight>
{{CodeLine5|0046}}<syntaxhighlight lang="lua">--end</syntaxhighlight>
{{CodeLine5|0047}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0874}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler(function(bHiding)</syntaxhighlight>
{{CodeLine5|0875}}<syntaxhighlight lang="lua">if(not bHiding) then</syntaxhighlight>
{{CodeLine5|0876}}<syntaxhighlight lang="lua">RefreshMods();</syntaxhighlight>
{{CodeLine5|0877}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0878}}<syntaxhighlight lang="lua">SetListingsState("results");</syntaxhighlight>
{{CodeLine5|0879}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0880}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0533}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler( ShowHideHandler )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0538}}<syntaxhighlight lang="lua">function AdjustScreenSize()</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsMenu.lua}}
:<code>UI/FrontEnd/Modding/ModsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler(function(isHiding)</syntaxhighlight>
{{CodeLine5|0039}}<syntaxhighlight lang="lua">if(not isHiding) then</syntaxhighlight>
{{CodeLine5|0040}}<syntaxhighlight lang="lua">local supportsSinglePlayer = Modding.AllEnabledModsContainPropertyValue("SupportsSinglePlayer", 1);</syntaxhighlight>
{{CodeLine5|0041}}<syntaxhighlight lang="lua">local supportsMultiplayer = Modding.AllEnabledModsContainPropertyValue("SupportsMultiplayer", 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">Controls.SinglePlayerButton:SetDisabled(not supportsSinglePlayer);</syntaxhighlight>
{{CodeLine5|0044}}<syntaxhighlight lang="lua">Controls.MultiPlayerButton:SetDisabled(not supportsMultiplayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">--if(supportsSinglePlayer and not supportsMultiplayer) then</syntaxhighlight>
{{CodeLine5|0047}}<syntaxhighlight lang="lua">--OnSinglePlayerClick();</syntaxhighlight>
{{CodeLine5|0048}}<syntaxhighlight lang="lua">--elseif(supportsMultiplayer and not supportsSinglePlayer) then</syntaxhighlight>
{{CodeLine5|0049}}<syntaxhighlight lang="lua">--OnMultiPlayerClick();</syntaxhighlight>
{{CodeLine5|0050}}<syntaxhighlight lang="lua">--end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">g_InstanceManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">local mods = Modding.GetEnabledModsByActivationOrder();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">if(#mods == 0) then</syntaxhighlight>
{{CodeLine5|0057}}<syntaxhighlight lang="lua">Controls.ModsInUseLabel:SetHide(true);</syntaxhighlight>
{{CodeLine5|0058}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0059}}<syntaxhighlight lang="lua">Controls.ModsInUseLabel:SetHide(false);</syntaxhighlight>
{{CodeLine5|0060}}<syntaxhighlight lang="lua">for i,v in ipairs(mods) do</syntaxhighlight>
{{CodeLine5|0061}}<syntaxhighlight lang="lua">   local displayName = Modding.GetModProperty(v.ModID, v.Version, "Name");</syntaxhighlight>
{{CodeLine5|0062}}<syntaxhighlight lang="lua">   local displayNameVersion = string.format("[ICON_BULLET] %s (v. %i)", displayName, v.Version);</syntaxhighlight>
{{CodeLine5|0063}}<syntaxhighlight lang="lua">   local listing = g_InstanceManager:GetInstance();</syntaxhighlight>
{{CodeLine5|0064}}<syntaxhighlight lang="lua">   listing.Label:SetText(displayNameVersion);</syntaxhighlight>
{{CodeLine5|0065}}<syntaxhighlight lang="lua">   listing.Label:SetToolTipString(displayNameVersion);</syntaxhighlight>
{{CodeLine5|0066}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0067}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0068}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0069}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsSinglePlayer.lua}}
:<code>UI/FrontEnd/Modding/ModsSinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler(function(isHiding)</syntaxhighlight>
{{CodeLine5|0047}}<syntaxhighlight lang="lua">if(not isHiding) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">local bHasCustomGames = false;</syntaxhighlight>
{{CodeLine5|0050}}<syntaxhighlight lang="lua">for row in Modding.GetActivatedModEntryPoints("Custom") do</syntaxhighlight>
{{CodeLine5|0051}}<syntaxhighlight lang="lua">   bHasCustomGames = true;</syntaxhighlight>
{{CodeLine5|0052}}<syntaxhighlight lang="lua">   break;</syntaxhighlight>
{{CodeLine5|0053}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">   Controls.PlayMapButton:SetHide(Modding.AnyEnabledModsContainPropertyValue("HideSetupGame", 1));</syntaxhighlight>
{{CodeLine5|0056}}<syntaxhighlight lang="lua">   Controls.CustomGameButton:SetHide(not bHasCustomGames);</syntaxhighlight>
{{CodeLine5|0057}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0058}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ScenariosMenu.lua}}
:<code>UI/FrontEnd/ScenariosMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler(function(isHide)</syntaxhighlight>
{{CodeLine5|0068}}<syntaxhighlight lang="lua">if( not isHide ) then</syntaxhighlight>
{{CodeLine5|0069}}<syntaxhighlight lang="lua">Modding.DeactivateMods();</syntaxhighlight>
{{CodeLine5|0070}}<syntaxhighlight lang="lua">SetupFileButtonList();</syntaxhighlight>
{{CodeLine5|0071}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0072}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0502}}<syntaxhighlight lang="lua">ContextPtr:SetShowHideHandler( OnShowHide );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetShowHideHandler]]
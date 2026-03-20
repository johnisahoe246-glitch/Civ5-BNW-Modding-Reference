{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|EditBox}}, {{Type5|Image}}, {{Type5|Label}} and '''TextBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' UIElement:GetText<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0909}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns(Controls.MaxTurnsEdit:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">if (PreGame.TestPassword( ePlayer, Controls.OldPasswordEditBox:GetText() ) ) then</syntaxhighlight>
{{CodeLine5|0010}}<syntaxhighlight lang="lua">if ( Controls.NewPasswordEditBox:GetText() == Controls.RetypeNewPasswordEditBox:GetText() ) then</syntaxhighlight>
{{CodeLine5|0011}}<syntaxhighlight lang="lua">PreGame.SetPassword( ePlayer, Controls.NewPasswordEditBox:GetText(), Controls.OldPasswordEditBox:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">if(   ValidateText(Controls.NewPasswordEditBox:GetText()) and</syntaxhighlight>
{{CodeLine5|0086}}<syntaxhighlight lang="lua">ValidateText(Controls.RetypeNewPasswordEditBox:GetText()) and</syntaxhighlight>
{{CodeLine5|0087}}<syntaxhighlight lang="lua">Controls.NewPasswordEditBox:GetText() == Controls.RetypeNewPasswordEditBox:GetText() and</syntaxhighlight>
{{CodeLine5|0088}}<syntaxhighlight lang="lua">PreGame.TestPassword( Game.GetActivePlayer(), Controls.OldPasswordEditBox:GetText() ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">local name = Controls.NewName:GetText();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6339}}<syntaxhighlight lang="lua">local searchString = Controls.SearchEditBox:GetText();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">local fromName = controlTable.String:GetText();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0158}}<syntaxhighlight lang="lua">toName = Locale.ConvertTextKey( "TXT_KEY_DIPLO_TO_PLAYER", controlTable.String:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0301}}<syntaxhighlight lang="lua">Controls.ChatPull:GetButton():SetText( Controls.LengthTest:GetText() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0615}}<syntaxhighlight lang="lua">local tooltip = v.Value.Label:GetText();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0743}}<syntaxhighlight lang="lua">PreGame.SetMaxTurns( Controls.MaxTurnsEdit:GetText() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">local strGameName = Controls.NameBox:GetText();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">if (PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText() )) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">local bValid = PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">local bValid = PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">local newSave = Controls.NameBox:GetText();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">UI.SaveMap( Controls.NameBox:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">local text = Controls.NameBox:GetText();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">UI.CopyLastAutoSave( Controls.NameBox:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0053}}<syntaxhighlight lang="lua">UI.SaveGame( Controls.NameBox:GetText() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCityName.lua}}
:<code>UI/InGame/Popups/SetCityName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Network.SendRenameCity(pCity:GetID(), Controls.EditCityName:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">if (Controls.EditCivLeader:GetText() ~= szDefaultPlayerLeader) then</syntaxhighlight>
{{CodeLine5|0050}}<syntaxhighlight lang="lua">PreGame.SetLeaderName( g_EditSlot, Controls.EditCivLeader:GetText());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">if (Controls.EditCivName:GetText() ~= szDefaultPlayerCiv) then</syntaxhighlight>
{{CodeLine5|0053}}<syntaxhighlight lang="lua">PreGame.SetCivilizationDescription( g_EditSlot, Controls.EditCivName:GetText());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">if (Controls.EditCivShortName:GetText() ~= szDefaultPlayerShortCiv) then</syntaxhighlight>
{{CodeLine5|0056}}<syntaxhighlight lang="lua">PreGame.SetCivilizationShortDescription( g_EditSlot, Controls.EditCivShortName:GetText());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">if (Controls.EditCivAdjective:GetText() ~= szDefaultPlayerCivAdjective) then</syntaxhighlight>
{{CodeLine5|0059}}<syntaxhighlight lang="lua">PreGame.SetCivilizationAdjective( g_EditSlot, Controls.EditCivAdjective:GetText());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">PreGame.SetNickName( g_EditSlot, Controls.EditNickName:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">PreGame.SetPassword( g_EditSlot, Controls.EditPassword:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">if(   ValidateText(Controls.EditCivShortName:GetText()) and</syntaxhighlight>
{{CodeLine5|0141}}<syntaxhighlight lang="lua">ValidateText(Controls.EditCivLeader:GetText()) and</syntaxhighlight>
{{CodeLine5|0142}}<syntaxhighlight lang="lua">ValidateText(Controls.EditCivName:GetText()) and</syntaxhighlight>
{{CodeLine5|0143}}<syntaxhighlight lang="lua">ValidateText(Controls.EditCivAdjective:GetText())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">if ( ValidateText( Controls.EditNickName:GetText()) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0150}}<syntaxhighlight lang="lua">if ( ValidateText(Controls.EditPassword:GetText() ) and</syntaxhighlight>
{{CodeLine5|0151}}<syntaxhighlight lang="lua">Controls.EditRetypePassword:GetText() ==  Controls.EditPassword:GetText() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">if (Controls.EditPassword:GetText() ~= "" or Controls.EditRetypePassword:GetText() ~= "") then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetUnitName.lua}}
:<code>UI/InGame/Popups/SetUnitName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Network.SendRenameUnit(pUnit:GetID(), Controls.EditUnitName:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SupportFunctions.lua}}
:<code>UI/SupportFunctions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0007}}<syntaxhighlight lang="lua">longStr = control:GetText();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">strPlayer = Controls.UNInfo:GetText();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0468}}<syntaxhighlight lang="lua">strCiv = Controls.CultureLabel:GetText();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0531}}<syntaxhighlight lang="lua">controlTable.Name:SetText(controlTable.Score:GetText());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetText]]
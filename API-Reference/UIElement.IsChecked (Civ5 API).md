{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|CheckBox}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:IsChecked<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0898}}<syntaxhighlight lang="lua">if(Controls.MaxTurnsCheck:IsChecked()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0920}}<syntaxhighlight lang="lua">Controls.MaxTurnsEditbox:SetHide(not Controls.MaxTurnsCheck:IsChecked());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorModal.lua}}
:<code>UI/InGame/Popups/AdvisorModal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">if (Controls.DontShowAgainCheckbox:IsChecked()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">if(g_TutorialQueue[1] ~= nil and Controls.DontShowAgainCheckbox:IsChecked()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0425}}<syntaxhighlight lang="lua">if( Controls.CreateRoad_Checkbox:IsChecked() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0783}}<syntaxhighlight lang="lua">if(Controls.DeleteUserData:IsChecked()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">local bChecked = Controls.PrivateGameCheckbox:IsChecked();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">if (Controls.VerboseLoggingToggle:IsChecked()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0499}}<syntaxhighlight lang="lua">local bUsingSteamCloud = Controls.CloudCheck:IsChecked();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0064}}<syntaxhighlight lang="lua">if ( Controls.UsePasswordCheck:IsChecked() ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsChecked]]
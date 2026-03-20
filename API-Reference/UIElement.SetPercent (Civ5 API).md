{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetPercent<b>(</b>'''int''' percentDone<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|percentDone:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0292}}<syntaxhighlight lang="lua">controls.GrowthBar:SetPercent( fGrowthProgressPercent );</syntaxhighlight>
{{CodeLine5|0293}}<syntaxhighlight lang="lua">controls.GrowthBarShadow:SetPercent( fGrowthProgressPlusThisTurnPercent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">controls.ProductionBar:SetPercent( fProductionProgressPercent );</syntaxhighlight>
{{CodeLine5|0315}}<syntaxhighlight lang="lua">controls.ProductionBarShadow:SetPercent( fProductionProgressPlusThisTurnPercent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0850}}<syntaxhighlight lang="lua">instance.SubControls.CityBannerHealthBar:SetPercent(iHealthPercent);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">instance.HealthBar:SetPercent( iHealthPercent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">instance.GrowthBar:SetPercent( fGrowthProgressPercent );</syntaxhighlight>
{{CodeLine5|0181}}<syntaxhighlight lang="lua">instance.GrowthBarShadow:SetPercent( fGrowthProgressPlusThisTurnPercent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">instance.ProductionBar:SetPercent( fProductionProgressPercent );</syntaxhighlight>
{{CodeLine5|0354}}<syntaxhighlight lang="lua">instance.ProductionBarShadow:SetPercent( fProductionProgressPlusThisTurnPercent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">Controls.StatusMeter:SetPercent(info.value);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">posBarCtrl:SetPercent(percentFull);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0124}}<syntaxhighlight lang="lua">negBarCtrl:SetPercent(percentFull);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0753}}<syntaxhighlight lang="lua">Controls.PeopleMeter:SetPercent( pCity:GetFood() / pCity:GrowthThreshold() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0976}}<syntaxhighlight lang="lua">controlTable.GPMeter:SetPercent( percent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1384}}<syntaxhighlight lang="lua">Controls.CultureMeter:SetPercent( percentComplete );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1494}}<syntaxhighlight lang="lua">Controls.HealthMeter:SetPercent(iHealthPercent);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0479}}<syntaxhighlight lang="lua">controlTable.StatusMeter:SetPercent(info.value);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0484}}<syntaxhighlight lang="lua">pStack.StatusMeter:SetPercent(info.value);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">instance.HealthBar:SetPercent( pct );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">instance.GPMeter:SetPercent( iProgress / iThreshold );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">Controls.GGMeter:SetPercent( fProgress / fThreshold );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">Controls.GAMeter:SetPercent( fProgress / fThreshold );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">Controls.GPMeter:SetPercent( fProgress / fThreshold );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">Controls.GrowthBar:SetPercent( city:GetFood() / city:GrowthThreshold() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">Controls.UtopiaBar:SetPercent( percentDone );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0436}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetPercent( healthPercent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">o.m_Instance.TargetColor:SetPercent( 100 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0375}}<syntaxhighlight lang="lua">Controls.WorkerProgressBar:SetPercent( percent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">Controls.XPMeter:SetPercent( iExperience / iExperienceNeeded );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0310}}<syntaxhighlight lang="lua">Controls.TechProgress:SetPercent(g_PreReqsAcquired / totalPreReqs);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPercent]]
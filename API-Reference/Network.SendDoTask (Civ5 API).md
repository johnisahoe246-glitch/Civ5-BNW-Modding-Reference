{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendDoTask<b>(</b>{{Type5|CityID}} cityID, {{Type5|TaskType}} task, '''int''' plotIndex, '''int''' arg3, '''bool''' arg4, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|cityID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|task:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plotIndex:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg4:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alt:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shift:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ctrl:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AnnexCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/AnnexCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">Network.SendDoTask(cityID, TaskTypes.TASK_ANNEX_PUPPET, -1, -1, false, false, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">Network.SendDoTask(pCity:GetID(), TaskTypes.TASK_CHANGE_WORKING_PLOT, 0, -1, false, bAlt, bShift, bCtrl);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1685}}<syntaxhighlight lang="lua">Network.SendDoTask(pCity:GetID(), TaskTypes.TASK_CHANGE_WORKING_PLOT, iPlotIndex, -1, false, bAlt, bShift, bCtrl);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2189}}<syntaxhighlight lang="lua">Network.SendDoTask(pCity:GetID(), TaskTypes.TASK_UNRAZE, -1, -1, false, false, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ConfirmCityTaskPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmCityTaskPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">Network.SendDoTask(iCityID, iTask, -1, -1, false, false, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LiberateMinorPopup.lua}}
:<code>UI/InGame/PopupsGeneric/LiberateMinorPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">Network.SendDoTask(iCityID, TaskTypes.TASK_CREATE_PUPPET, -1, -1, false, false, false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PuppetCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/PuppetCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">Network.SendDoTask(cityID, TaskTypes.TASK_CREATE_PUPPET, -1, -1, false, false, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">Network.SendDoTask(cityID, TaskTypes.TASK_RAZE, -1, -1, false, false, false, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendDoTask]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetProjectProductionTurnsLeft<b>(</b>{{Type5|ProjectType}} project, '''int''' num<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|project:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|num:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">Controls[controlTurns]:SetText(  Locale.ConvertTextKey("TXT_KEY_PRODUCTION_HELP_NUM_TURNS",city:GetProjectProductionTurnsLeft(queuedData1, queuedItemNumber-1)) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">strTurnsLeft = Locale.ConvertTextKey( "TXT_KEY_STR_TURNS", city:GetProjectProductionTurnsLeft( projectID ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0707}}<syntaxhighlight lang="lua">Controls[controlTurns]:SetText( Locale.ConvertTextKey("TXT_KEY_PRODUCTION_HELP_NUM_TURNS", city:GetProjectProductionTurnsLeft(queuedData1, i-1)) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProjectProductionTurnsLeft]]
[[Category:Civ5 City Production API|GetProjectProductionTurnsLeft]]
[[Category:Civ5 Buildings API|GetProjectProductionTurnsLeft]]
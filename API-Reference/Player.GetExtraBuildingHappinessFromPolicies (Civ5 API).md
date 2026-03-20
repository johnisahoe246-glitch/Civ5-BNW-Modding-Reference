{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetExtraBuildingHappinessFromPolicies<b>(</b>{{Type5|PlayerID}} building<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">iHappinessTotal = iHappinessTotal + pActivePlayer:GetExtraBuildingHappinessFromPolicies(iBuildingID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetExtraBuildingHappinessFromPolicies]]
[[Category:Civ5 Buildings API|GetExtraBuildingHappinessFromPolicies]]
[[Category:Civ5 Happiness API|GetExtraBuildingHappinessFromPolicies]]
[[Category:Civ5 Policies API|GetExtraBuildingHappinessFromPolicies]]
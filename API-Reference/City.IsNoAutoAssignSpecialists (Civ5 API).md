{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:IsNoAutoAssignSpecialists<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0640}}<syntaxhighlight lang="lua">Controls.NoAutoSpecialistCheckbox:SetCheck(pCity:IsNoAutoAssignSpecialists());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1975}}<syntaxhighlight lang="lua">if (not UI.GetHeadSelectedCity():IsNoAutoAssignSpecialists()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2034}}<syntaxhighlight lang="lua">if (not pCity:IsNoAutoAssignSpecialists()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsNoAutoAssignSpecialists]]
[[Category:Civ5 Specialists API|IsNoAutoAssignSpecialists]]
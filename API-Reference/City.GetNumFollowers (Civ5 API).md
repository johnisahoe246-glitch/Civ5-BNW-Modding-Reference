{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetNumFollowers<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1122}}<syntaxhighlight lang="lua">local iFollowers = city:GetNumFollowers(eReligion)</syntaxhighlight>
{{CodeLine5|1123}}<syntaxhighlight lang="lua">if (not bFirst) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1135}}<syntaxhighlight lang="lua">if (iReligionID >= 0 and iReligionID ~= eReligion and city:GetNumFollowers(iReligionID) > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1156}}<syntaxhighlight lang="lua">local iFollowers = city:GetNumFollowers(iReligionID)</syntaxhighlight>
{{CodeLine5|1157}}<syntaxhighlight lang="lua">if (not bFirst) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumFollowers]]
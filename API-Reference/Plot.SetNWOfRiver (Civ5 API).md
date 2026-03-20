{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Plot:SetNWOfRiver<b>(</b>'''bool''' newValue<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0471}}<syntaxhighlight lang="lua">riverPlot:SetNWOfRiver(true, thisFlowDirection);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetNWOfRiver]]
[[Category:Civ5 Rivers API|SetNWOfRiver]]
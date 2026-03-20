{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' Modding.PublishedFileIdsMatch<b>(</b>'''unknown''' arg0, '''unknown''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">if(not Modding.PublishedFileIdsMatch(v.PublishedFileId, downloadingFiles[i].PublishedFileId)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PublishedFileIdsMatch]]
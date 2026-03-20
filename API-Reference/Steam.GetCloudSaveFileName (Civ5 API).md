{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Obtains the fully qualified filename of a Cloud Save slot


=Usage=
<code>'''string''' Steam.GetCloudSaveFileName<b>(</b>'''int''' slot<b>)</b></code>


'''Returned Value'''
:Returns the fully qualified filename of a Cloud Save slot.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|slot:
|valign="top"| ''An integer pertaining to the cloud save slot.
Must be between 1 and Steam.GetMaxCloudSaves()''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
--Load a cloud save
Events.PlayerChoseToLoadGame(Steam.GetCloudSaveFileName(g_iSelected), true);</syntaxhighlight>


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">Events.PlayerChoseToLoadGame(Steam.GetCloudSaveFileName(g_iSelected), true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">local thisLoadFile = Steam.GetCloudSaveFileName(g_iSelected);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCloudSaveFileName]]
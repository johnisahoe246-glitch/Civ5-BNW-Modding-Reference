{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' OptionsManager.GetTooltip2Seconds<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0093}}<syntaxhighlight lang="lua">if( m_fTime > (OptionsManager.GetTooltip2Seconds() / 100) ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTooltip2Seconds]]
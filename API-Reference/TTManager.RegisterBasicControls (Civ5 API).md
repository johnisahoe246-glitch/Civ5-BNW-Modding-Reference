{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|TTManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' TTManager.RegisterBasicControls<b>(</b>{{Type5|AlphaAnim}} arg0, {{Type5|SlideAnim}} arg1, {{Type5|Label}} arg2, {{Type5|Grid}} arg3<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ToolTips.lua}}
:<code>UI/FrontEnd/ToolTips.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">TTManager:RegisterBasicControls( Controls.ToolTipRoot, Controls.ToolTipStore, Controls.ToolTipText, Controls.ToolTipGrid );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RegisterBasicControls]]
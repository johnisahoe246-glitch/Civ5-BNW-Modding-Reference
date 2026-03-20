{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|WorldAnchor}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetWorldPositionVal<b>(</b>'''int''' worldPosX, '''int''' worldPosY, '''int''' worldPosZ<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|worldPosX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|worldPosY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|worldPosZ:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|PathHelpManager.lua}}
:<code>UI/InGame/WorldView/PathHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">instance.Anchor:SetWorldPositionVal( worldPosX, worldPosY, worldPosZ );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">instance.Anchor:SetWorldPositionVal( x + g_ResourceIconOffsetX,</syntaxhighlight>
{{CodeLine5|0055}}<syntaxhighlight lang="lua">y + g_ResourceIconOffsetY,</syntaxhighlight>
{{CodeLine5|0056}}<syntaxhighlight lang="lua">z + g_ResourceIconOffsetZ );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0819}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:SetWorldPositionVal( posX, posY, posZ );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetWorldPositionVal]]
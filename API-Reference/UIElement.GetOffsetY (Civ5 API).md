{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:GetOffsetY<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">local newSizeY = sizeY + controlTable.OuterStack:GetOffsetY()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0296}}<syntaxhighlight lang="lua">controlTable.Button:SetSizeY(newSizeY);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">local TOP_COMPENSATION = Controls.OuterGrid:GetOffsetY();</syntaxhighlight>
{{CodeLine5|0032}}<syntaxhighlight lang="lua">local PANEL_OFFSET = Controls.ScrollPanel:GetOffsetY() + 48;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0328}}<syntaxhighlight lang="lua">yAbsoluteOffset = yAbsoluteOffset + Controls.GraphsPanel:GetOffsetY() + Controls.GraphDisplay:GetOffsetY();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetOffsetY]]
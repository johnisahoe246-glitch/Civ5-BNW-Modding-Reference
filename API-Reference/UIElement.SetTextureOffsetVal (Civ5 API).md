{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetTextureOffsetVal<b>(</b>'''int''' arg0, '''int''' offset<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|offset:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua (G&K)}}
:<code>DLC/Expansion/UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1817}}<syntaxhighlight lang="lua">Controls.Portrait:SetTextureOffsetVal(0,0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">imageControl:SetTextureOffsetVal( (offset % numCols) * iconSize, math.floor(offset / numCols) * iconSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">teamColorControl:SetTextureOffsetVal( 141, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">teamColorControl:SetTextureOffsetVal( 77, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">teamColorControl:SetTextureOffsetVal( 32, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">teamColorControl:SetTextureOffsetVal( 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0239}}<syntaxhighlight lang="lua">instance.MovementPip:SetTextureOffsetVal( 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0241}}<syntaxhighlight lang="lua">instance.MovementPip:SetTextureOffsetVal( 0, 96 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0243}}<syntaxhighlight lang="lua">instance.MovementPip:SetTextureOffsetVal( 0, 32 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">controlTable.Icon:SetTextureOffsetVal( 228, 68 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TaskList.lua}}
:<code>UI/InGame/TaskList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">controlTable.TaskEntryImage:SetTextureOffsetVal(0, iOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">imageInstance.Image:SetTextureOffsetVal( yieldType * 128, 512 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">imageInstance.Image:SetTextureOffsetVal( yieldType * 128, 128 * ( amount - 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">textImageInstance.Image:SetTextureOffsetVal( GetNumberOffset( amount ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0150}}<syntaxhighlight lang="lua">imageInstance.Image:SetTextureOffsetVal( 0 * 128, 512 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">imageInstance.Image:SetTextureOffsetVal( 0 * 128, 128 * ( amount - 1 ) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetTextureOffsetVal]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetColorVal<b>(</b>'''int''' arg0, '''int''' arg1 = nil, '''int''' arg2 = nil, '''int''' arg3 = nil<b>)</b></code>


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
''Redundant occurences have been removed.''

{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">itemInstance.Box:SetColorVal(unpack(ltBlue));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">itemInstance.Box:SetColorVal(unpack(dkBlue));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0555}}<syntaxhighlight lang="lua">agentEntry.Base:SetColorVal(0,0,0,0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0566}}<syntaxhighlight lang="lua">agentEntry.Base:SetColorVal(unpack(bTickTock and g_PianoKeys[0] or g_PianoKeys[1]));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0973}}<syntaxhighlight lang="lua">entry.Base:SetColorVal(unpack(bTickTock and g_PianoKeys[0] or g_PianoKeys[1]));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1476}}<syntaxhighlight lang="lua">instance.Base:SetColorVal(unpack(bTickTock and g_PianoKeys[0] or g_PianoKeys[1]));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">lineSegment.LineSegment:SetColorVal(color.Red, color.Green, color.Blue, color.Alpha);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0719}}<syntaxhighlight lang="lua">graphLegendInstance.LegendLine:SetColorVal(color.Red, color.Green, color.Blue, color.Alpha);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetColorVal]]
[[Category:Civ5 Players API|SetColorVal]]
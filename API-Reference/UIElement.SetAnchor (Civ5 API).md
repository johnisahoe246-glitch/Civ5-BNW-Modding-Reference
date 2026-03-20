{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetAnchor<b>(</b>'''string''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">Controls.ReligionStack:SetAnchor("L,T");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">Controls.ReligionStack:SetAnchor("C,T");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">instance.UnitActionButton:SetAnchor( "L,B" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">Controls.WonderSplash:SetAnchor( thisBuilding.WonderSplashAnchor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">Controls.WonderSplash:SetAnchor( "T,R" );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetAnchor]]
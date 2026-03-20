{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:ChangeParent<b>(</b>{{Type5|Image}} parent<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|parent:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:ChangeParent( g_SelectedContainer );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:ChangeParent( Controls.AirCraftFlags );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0466}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:ChangeParent( Controls.CivilianFlags );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0468}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:ChangeParent( Controls.GarrisonFlags );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0470}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:ChangeParent( Controls.MilitaryFlags );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1550}}<syntaxhighlight lang="lua">g_SelectedFlag.m_Instance.Anchor:ChangeParent( Controls.MilitaryFlags );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">record.AnchorInstance.Anchor:ChangeParent( Controls.YieldStore );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">imageInstance.Image:ChangeParent( parent );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">textImageInstance.Image:ChangeParent( imageInstance.Image );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">instance.Anchor:ChangeParent( Controls.Scrap );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">instance.Image:ChangeParent( Controls.Scrap );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeParent]]
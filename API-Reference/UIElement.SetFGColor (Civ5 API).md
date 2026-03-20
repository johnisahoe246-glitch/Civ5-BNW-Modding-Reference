{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Bar}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetFGColor<b>(</b>{{Type5|Vector4}} tBarColor<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tBarColor:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0860}}<syntaxhighlight lang="lua">instance.SubControls.CityBannerHealthBar:SetFGColor( tBarColor );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">instance.HealthBar:SetFGColor( { x = 0, y = 1, z = 0, w = 1 } );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">instance.HealthBar:SetFGColor( { x = 1, y = 1, z = 0, w = 1 } );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">instance.HealthBar:SetFGColor( { x = 1, y = 0, z = 0, w = 1 } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetFGColor( Vector4( 0, 1, 0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetFGColor( Vector4( 1, 1, 0, 1 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0409}}<syntaxhighlight lang="lua">self.m_Instance.HealthBar:SetFGColor( Vector4( 1, 0, 0, 1 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">self.m_Instance.TargetColor:SetFGColor( color );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetFGColor]]
[[Category:Civ5 Players API|SetFGColor]]
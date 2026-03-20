{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:IsForcedAvoidGrowth<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0948}}<syntaxhighlight lang="lua">Controls.AvoidGrowthButton:SetCheck( pCity:IsForcedAvoidGrowth() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2294}}<syntaxhighlight lang="lua">Network.SendSetCityAvoidGrowth( pCity:GetID(), not pCity:IsForcedAvoidGrowth() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsForcedAvoidGrowth]]
[[Category:Civ5 Food & Population API|IsForcedAvoidGrowth]]
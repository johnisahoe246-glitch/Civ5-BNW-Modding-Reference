{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsCargo<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0709}}<syntaxhighlight lang="lua">if( pPlotUnit:IsCargo() and pPlotUnit:GetTransportUnit():GetID() == self.m_UnitID ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0759}}<syntaxhighlight lang="lua">if( pUnit:IsCargo() and self.m_CarrierFlag ~= nil ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0986}}<syntaxhighlight lang="lua">if( thisUnit:IsCargo() ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCargo]]
[[Category:Civ5 Movement API|IsCargo]]
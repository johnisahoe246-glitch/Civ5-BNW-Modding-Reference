{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsDead<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0885}}<syntaxhighlight lang="lua">Players[ playerID ]:GetUnitByID( unitID ):IsDead() )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">if( test ~= nil and test:GetID() ~= self.m_UnitID and not test:IsGarrisoned() and not test:IsDead() and not test:IsDelayedDeath() )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0252}}<syntaxhighlight lang="lua">if ( unit == nil or unit:IsDead() ) then return end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0540}}<syntaxhighlight lang="lua">if (unit == nil or unit:IsDead() ) then return end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsDead]]
[[Category:Civ5 Combat API|IsDead]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:CargoSpace<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">if( pUnit:CargoSpace() > 0 ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0668}}<syntaxhighlight lang="lua">if( pUnit:CargoSpace() <= 0 ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CargoSpace]]
[[Category:Civ5 Movement API|CargoSpace]]
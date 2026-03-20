{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' PreGame.IsEarthMap<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0630}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:GetButton():SetDisabled(not bIsMapScript and not PreGame.IsEarthMap());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0837}}<syntaxhighlight lang="lua">if(PreGame.IsEarthMap()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsEarthMap]]
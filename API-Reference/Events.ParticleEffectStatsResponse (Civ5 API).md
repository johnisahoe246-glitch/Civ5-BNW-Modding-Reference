{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.ParticleEffectStatsResponse<b>(</b>'''unknown''' responseData<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ParticleEffectStatsResponse.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ParticleEffectStatsResponse(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|responseData:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0253}}<syntaxhighlight lang="lua">Events.ParticleEffectStatsResponse.Add( OnPEffectStatsResponse );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ParticleEffectStatsResponse]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Plot:CanHaveResource<b>(</b>{{Type5|ResourceType}} resource, '''bool''' ignoreLatitude<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ignoreLatitude:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">if (plot:CanHaveResource(resource.ID, ignoreLatitude)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">if (not plot:CanHaveResource(resourceID, ignoreLatitude)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanHaveResource]]
[[Category:Civ5 Resources API|CanHaveResource]]
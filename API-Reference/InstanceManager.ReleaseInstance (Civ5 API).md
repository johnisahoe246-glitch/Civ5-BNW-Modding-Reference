{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|InstanceManager}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' InstanceManager:ReleaseInstance<b>(</b>'''table''' instance<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|instance:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0674}}<syntaxhighlight lang="lua">g_TeamIM:ReleaseInstance( instance.SubControls );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0679}}<syntaxhighlight lang="lua">g_SVStrikeIM:ReleaseInstance( svInstance );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0691}}<syntaxhighlight lang="lua">g_OtherIM:ReleaseInstance( instance.SubControls );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0819}}<syntaxhighlight lang="lua">g_OtherIM:ReleaseInstance( banner.SubControls );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0821}}<syntaxhighlight lang="lua">g_TeamIM:ReleaseInstance( banner.SubControls );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0938}}<syntaxhighlight lang="lua">g_PopupIM:ReleaseInstance( instance );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0949}}<syntaxhighlight lang="lua">g_PopupIM:ReleaseInstance( v );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">g_ResourceManager:ReleaseInstance( instance );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">g_AnchorIM:ReleaseInstance( instance );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">g_ImageIM:ReleaseInstance( instance );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ReleaseInstance]]
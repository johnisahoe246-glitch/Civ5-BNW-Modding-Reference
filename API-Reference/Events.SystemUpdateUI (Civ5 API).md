{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SystemUpdateUI<b>(</b>{{Type5|SystemUpdateUIType}} type<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SystemUpdateUI.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SystemUpdateUI(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|type:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1315}}<syntaxhighlight lang="lua">Events.SystemUpdateUI.Add( OnUpdateUI );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6432}}<syntaxhighlight lang="lua">Events.SystemUpdateUI.CallImmediate( SystemUpdateUIType.BulkShowUI );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6434}}<syntaxhighlight lang="lua">Events.SystemUpdateUI.CallImmediate( SystemUpdateUIType.BulkHideUI );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1070}}<syntaxhighlight lang="lua">Events.SystemUpdateUI.Add( SystemUpdateUIHandler )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1073}}<syntaxhighlight lang="lua">function ShowHideHandler( bIsHide )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0507}}<syntaxhighlight lang="lua">Events.SystemUpdateUI( SystemUpdateUIType.ReloadUI );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SystemUpdateUI]]
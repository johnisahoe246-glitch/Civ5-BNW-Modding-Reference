{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|EditBox}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:TakeFocus<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">Controls.OldPasswordEditBox:TakeFocus();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0241}}<syntaxhighlight lang="lua">Controls.ChatEntry:TakeFocus();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Controls.EnterPasswordEditBox:TakeFocus();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">Controls.NameBox:TakeFocus();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0281}}<syntaxhighlight lang="lua">Controls.EditNickName:TakeFocus();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">Controls.EditCivLeader:TakeFocus();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">Controls.EditBox:TakeFocus();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TakeFocus]]
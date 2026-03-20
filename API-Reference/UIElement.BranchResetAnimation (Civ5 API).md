{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:BranchResetAnimation<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0917}}<syntaxhighlight lang="lua">instance.Anchor:BranchResetAnimation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewTurn.lua}}
:<code>UI/InGame/NewTurn.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">Controls.Anim:BranchResetAnimation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">root:BranchResetAnimation();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|BranchResetAnimation]]
[[Category:Civ5 Policies API|BranchResetAnimation]]
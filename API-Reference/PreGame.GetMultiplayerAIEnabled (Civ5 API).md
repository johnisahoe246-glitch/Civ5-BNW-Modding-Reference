{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' PreGame.GetMultiplayerAIEnabled<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">if(PreGame:GetMultiplayerAIEnabled()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1224}}<syntaxhighlight lang="lua">local bCanEnableAISlots = PreGame.GetMultiplayerAIEnabled();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMultiplayerAIEnabled]]
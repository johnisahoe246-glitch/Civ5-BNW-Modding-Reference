{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SequenceGameInitComplete<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SequenceGameInitComplete.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SequenceGameInitComplete(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|LoadScreen.lua}}
:<code>UI/FrontEnd/LoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">Events.SequenceGameInitComplete.Add( OnSequenceGameInitComplete );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0640}}<syntaxhighlight lang="lua">Events.SequenceGameInitComplete.Remove(InitializeTutorialSystem); -- only call this once</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0657}}<syntaxhighlight lang="lua">Events.SequenceGameInitComplete.Add(InitializeTutorialSystem)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0659}}<syntaxhighlight lang="lua">LuaEvents.TryQueueTutorial.Add(function(tutorialID, highPriority)</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SequenceGameInitComplete]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.EventPoliciesDirty<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.EventPoliciesDirty.Add(''<function handler>'')</code> or invoke it directly through <code>Events.EventPoliciesDirty(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">Events.EventPoliciesDirty.Add( UpdateDisplay );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0552}}<syntaxhighlight lang="lua">Events.EventPoliciesDirty();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EventPoliciesDirty]]
[[Category:Civ5 Policies API|EventPoliciesDirty]]
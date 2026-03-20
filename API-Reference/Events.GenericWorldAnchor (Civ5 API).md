{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.GenericWorldAnchor<b>(</b>{{Type5|GenericWorldAnchorType}} type, '''bool''' show, '''int''' plotX, '''int''' plotY, {{Type5|FeatureType}} data1 = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.GenericWorldAnchor.Add(''<function handler>'')</code> or invoke it directly through <code>Events.GenericWorldAnchor(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|type:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|show:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plotX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plotY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|data1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">Events.GenericWorldAnchor.Add( OnGenericWorldAnchor );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">Events.GenericWorldAnchor( GenericWorldAnchorTypes.WORLD_ANCHOR_WORKER, false, v.plot:GetX(), v.plot:GetY(), v.buildType );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0315}}<syntaxhighlight lang="lua">Events.GenericWorldAnchor( GenericWorldAnchorTypes.WORLD_ANCHOR_SETTLER, false, v:GetX(), v:GetY(), -1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">Events.GenericWorldAnchor( GenericWorldAnchorTypes.WORLD_ANCHOR_WORKER, true, v.plot:GetX(), v.plot:GetY(), v.buildType );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0361}}<syntaxhighlight lang="lua">Events.GenericWorldAnchor( GenericWorldAnchorTypes.WORLD_ANCHOR_SETTLER, true, v:GetX(), v:GetY(), -1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0852}}<syntaxhighlight lang="lua">Events.GenericWorldAnchor( GenericWorldAnchorTypes.WORLD_ANCHOR_SETTLER, false, v:GetX(), v:GetY() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GenericWorldAnchor]]
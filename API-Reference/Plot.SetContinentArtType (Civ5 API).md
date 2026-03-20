{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Plot:SetContinentArtType<b>(</b>{{Type5|ArtStyleType}} style<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|style:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1575}}<syntaxhighlight lang="lua">plot:SetContinentArtType(0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1577}}<syntaxhighlight lang="lua">plot:SetContinentArtType(3);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1610}}<syntaxhighlight lang="lua">plot:SetContinentArtType(1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetContinentArtType]]
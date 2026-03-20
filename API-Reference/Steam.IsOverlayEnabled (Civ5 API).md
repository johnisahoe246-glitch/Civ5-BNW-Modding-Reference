{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Determines if the Steam overlay is currently being displayed


=Usage=
<code>'''bool''' Steam.IsOverlayEnabled<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns true if the overlay is enabled, false if not.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local overlayEnabled = Steam.IsOverlayEnabled();
if(not overlayEnabled) then
-- show popups
else
-- wait
end</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsOverlayEnabled]]
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Opens the built-in web browser of the overlay and navigates to a store page on Steam


=Usage=
<code>'''void''' Steam.ActivateGameOverlayToStore<b>(</b>'''int''' storeID = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|storeID:
|valign="top"| ''Navigates the browser to the store page of the item with the given ID.
If no storeID is supplied, will navigate to the Civ5 store page.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
-- Open Civ5 Store page
Steam.ActivateGameOverlayToStore();</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MainMenu.lua}}
:<code>UI/FrontEnd/MainMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">Steam.ActivateGameOverlayToStore();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ActivateGameOverlayToStore]]
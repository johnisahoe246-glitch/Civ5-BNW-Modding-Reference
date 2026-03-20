{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumResourceAvailable<b>(</b>{{Type5|ResourceType}} resource, '''bool''' includeImport<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|includeImport:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0337}}<syntaxhighlight lang="lua">local iResourceCount = Players[iPlayer]:GetNumResourceAvailable( i, false );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">if (pPlayer:GetNumResourceAvailable(iResource) == 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">iAvailable = pPlayer:GetNumResourceAvailable( iResource, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">iNumAvailable = pPlayer:GetNumResourceAvailable(iResourceLoop, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1368}}<syntaxhighlight lang="lua">iResourceCount = g_pUs:GetNumResourceAvailable( resType, false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1435}}<syntaxhighlight lang="lua">iResourceCount = g_pThem:GetNumResourceAvailable( resType, false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2226}}<syntaxhighlight lang="lua">if (iAmount > Players[g_iUs]:GetNumResourceAvailable(resourceId, false)) then</syntaxhighlight>
{{CodeLine5|2227}}<syntaxhighlight lang="lua">iAmount = Players[g_iUs]:GetNumResourceAvailable(resourceId, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2231}}<syntaxhighlight lang="lua">if (iAmount > Players[g_iThem]:GetNumResourceAvailable(resourceId, false)) then</syntaxhighlight>
{{CodeLine5|2232}}<syntaxhighlight lang="lua">iAmount = Players[g_iThem]:GetNumResourceAvailable(resourceId, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2331}}<syntaxhighlight lang="lua">if (iNumResource > pPlayer:GetNumResourceAvailable(iResourceID, false)) then</syntaxhighlight>
{{CodeLine5|2332}}<syntaxhighlight lang="lua">iNumResource = pPlayer:GetNumResourceAvailable(iResourceID, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2792}}<syntaxhighlight lang="lua">local amount = pPlayer:GetNumResourceAvailable(iResourceLoop, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2816}}<syntaxhighlight lang="lua">if (pOtherPlayer:GetNumResourceAvailable(tradeableResource, true) == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2821}}<syntaxhighlight lang="lua">if(pOtherPlayer:GetNumResourceAvailable(tradeableResource, false) > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0994}}<syntaxhighlight lang="lua">if (iNumResourceNeededToUpgrade > 0 and iNumResourceNeededToUpgrade > pActivePlayer:GetNumResourceAvailable(iResourceLoop)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResourceAvailable]]
[[Category:Civ5 Resources API|GetNumResourceAvailable]]
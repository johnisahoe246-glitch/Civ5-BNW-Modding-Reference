{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


Triggers a notification for a Player. Notifications appear as icons on the right side of the screen.


=Usage=
<code>'''void''' Player:AddNotification<b>(</b>{{Type5|NotificationType}} notificationType, '''string''' description, '''string''' title, '''int''' x = -1, '''int''' y = -1, {{Type5|PlayerID}} extra1 = -1, '''int''' extra2 = -1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|notificationType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|description:
|valign="top"| ''The text displayed when mousing over the icon''
|-
|valign="top" style="padding-right:6px;"|title:
|valign="top"| ''The text displayed (temporarily) next to the icon''
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''X coordinate of relevant plot; use -1 if notification is not tied to a specific location''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''Y coordinate of relevant plot; use -1 if notification is not tied to a specific location''
|-
|valign="top" style="padding-right:6px;"|extra1:
|valign="top"| ''Optional additional information needed by some notification types''
|-
|valign="top" style="padding-right:6px;"|extra2:
|valign="top"| ''Optional additional information needed by some notification types''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local pPlayer = Players[Game.GetActivePlayer()]
local pCity = pPlayer:GetCapitalCity()
local sTitle = "Plague strikes " .. pCity:GetName()
local sText = pCity:GetName() .. " is suffering from plague; population has been decreased"
pPlayer:AddNotification(NotificationTypes.NOTIFICATION_STARVING, sText, sTitle, pCity:GetX(), pCity:GetY())</syntaxhighlight>


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">player:AddNotification(NotificationTypes.NOTIFICATION_GENERIC, text, heading);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0422}}<syntaxhighlight lang="lua">pPlayer:AddNotification(NotificationTypes.NOTIFICATION_GENERIC, text, heading);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0365}}<syntaxhighlight lang="lua">pActivePlayer:AddNotification(NotificationTypes.NOTIFICATION_GENERIC, sMessage, sSummary, -1, -1, iNewOwner);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddNotification]]
[[Category:Civ5 Notification API|AddNotification]]
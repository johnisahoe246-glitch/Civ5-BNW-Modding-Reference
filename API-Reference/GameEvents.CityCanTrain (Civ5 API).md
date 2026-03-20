{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}

This works exactly the same as {{FuncLabel5|GameEvents|CityCanConstruct}} but for units instead. Note however that the prerequisites for training units that are defined in the XML files have to be met before this event fires. Thus this event can be used to hide units that would otherwise be shown but not the other way around. Also, this event does not allow to restrict purchasing units with faith.

=Usage=
<code>'''void''' GameEvents.CityCanTrain<b>(</b>{{Type5|PlayerID}} player, {{Type5|CityID}} city, {{Type5|UnitType}} unitType<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''the index identifying the player who might or might not be able to construct''
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''the index identifying the city that might or might not be able to construct''
|-
|valign="top" style="padding-right:6px;"|buildingType:
|valign="top"| ''the ID of the unit that might or might not be able to be constructed''
|}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CityCanConstruct]]
[[Category:Civ5 Cities API|CityCanConstruct]]
[[Category:Civ5 City Production API|CityCanConstruct]]
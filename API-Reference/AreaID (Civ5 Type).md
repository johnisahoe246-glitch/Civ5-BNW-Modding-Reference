{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>AreaID</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!}}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
OBTAINLANDMASSBOUNDARIES
-->
|-
|align="right" width="200" |<code>table('''int''' => '''int''')</code>
|style="padding-left:6px" |<code>{{Func5|ObtainLandmassBoundaries}}<b>(</b>{{Type5|AreaID}} areaID<b>)</b></code>
<!-- 
GETID
-->
|-
|align="right" width="200" |<code>{{Type5|AreaID}}</code>
|style="padding-left:6px" |<code>{{Type5|Area}}:{{Func5|Area|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CANPLACECITYSTATEAT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|CanPlaceCityStateAt}}<b>(</b>'''int''' x, '''int''' y, {{Type5|AreaID}} area_ID, '''int''' force_it, '''int''' ignore_collisions<b>)</b></code>
<!-- 
CHOPINTOTHREEREGIONS
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|ChopIntoThreeRegions}}<b>(</b>'''unknown''' fertility_table, '''table''' rectangle_data_table, '''bool''' taller, '''unknown''' chopPercent = nil<b>)</b></code>
<!-- 
CHOPINTOTWOREGIONS
-->
|-
|align="right" width="200" |<code>'''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|ChopIntoTwoRegions}}<b>(</b>'''unknown''' fertility_table, '''table''' rectangle_data_table, '''bool''' taller, '''float''' chopPercent<b>)</b></code>
<!-- 
DIVIDEINTOREGIONS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|DivideIntoRegions}}<b>(</b>'''int''' numDivisions, '''unknown''' fertility_table, '''table''' rectangle_data_table<b>)</b></code>
<!-- 
MEASURESTARTPLACEMENTFERTILITYOFLANDMASS
-->
|-
|align="right" width="200" |<code>'''unknown''', {{Type5|AreaID}}, {{Type5|AreaID}}</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|MeasureStartPlacementFertilityOfLandmass}}<b>(</b>{{Type5|AreaID}} areaID, {{Type5|AreaID}} westX, '''int''' eastX, {{Type5|AreaID}} southY, '''int''' northY, '''bool''' wrapsX, '''bool''' wrapsY<b>)</b></code>
<!-- 
OBTAINNEXTSECTIONINREGION
-->
|-
|align="right" width="200" |<code>table('''int''' => '''int'''), table('''int''' => '''int'''), '''unknown''', '''unknown''', '''unknown''', '''unknown''', '''unknown'''</code>
|style="padding-left:6px" |<code>{{Type5|AssignStartingPlots}}:{{Func5|AssignStartingPlots|ObtainNextSectionInRegion}}<b>(</b>'''int''' incoming_west_x, '''int''' incoming_south_y, '''int''' incoming_width, '''int''' incoming_height, {{Type5|AreaID}} areaID, '''int''' force_it, '''int''' ignore_collisions<b>)</b></code>
<!-- 
AREAS
-->
|-
|align="right" width="200" |<code>iterator({{Type5|AreaID}}, {{Type5|Area}})</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|Areas}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAREA
-->
|-
|align="right" width="200" |<code>{{Type5|Area}}</code>
|style="padding-left:6px" |<code>{{Type5|Map}}.{{Func5|Map|GetArea}}<b>(</b>{{Type5|AreaID}} areaID<b>)</b></code>
<!-- 
GETAREA
-->
|-
|align="right" width="200" |<code>{{Type5|AreaID}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetArea}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNEARESTLANDAREA
-->
|-
|align="right" width="200" |<code>{{Type5|AreaID}}</code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|GetNearestLandArea}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETAREA
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Plot}}:{{Func5|Plot|SetArea}}<b>(</b>{{Type5|AreaID}} area<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|AreaID]]
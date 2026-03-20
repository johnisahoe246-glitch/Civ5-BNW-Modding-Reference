{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Map.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
==A==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
AREAS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>iterator({{Type5|AreaID}}, {{Type5|Area}})</code>
|width="100%" |<code>{{FuncLabel5|Map|Areas}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==C==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CALCULATEAREAS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Map|CalculateAreas}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CHANGEAIMAPHINT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Map|ChangeAIMapHint}}<b>(</b>'''int''' oneForNavalExpansion<b>)</b></code>
|}

==D==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
DEFAULTCONTINENTSTAMPER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Map|DefaultContinentStamper}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DOPLACENATURALWONDERS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|DoPlaceNaturalWonders}}<!-- No arguments --></code>
|}

==F==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
FINDBIGGESTAREA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Area}}</code>
|width="100%" |<code>{{FuncLabel5|Map|FindBiggestArea}}<b>(</b>'''bool''' ocean<b>)</b></code>
<!-- 
FINDWATER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Map|FindWater}}<b>(</b>{{Type5|Plot}} plot, '''int''' range, '''bool''' isFreshWater<b>)</b></code>
|}

==G==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETAIMAPHINT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetAIMapHint}}<!-- No arguments --></code>
<!-- 
GETAREA
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Area}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetArea}}<b>(</b>{{Type5|AreaID}} areaID<b>)</b></code>
<!-- 
GETCLIMATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ClimateType}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetClimate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETCUSTOMOPTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|GetCustomOption}}<b>(</b>'''int''' optionIndex<b>)</b></code>
<!-- 
GETFRACTALFLAGS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|GetFractalFlags}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETGRIDSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|GetGridSize}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINDEXAFTERLASTAREA
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetIndexAfterLastArea}}<!-- No arguments --></code>
<!-- 
GETLANDPLOTS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetLandPlots}}<!-- No arguments --></code>
<!-- 
GETNUMAREAS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetNumAreas}}<!-- No arguments --></code>
<!-- 
GETNUMLANDAREAS
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetNumLandAreas}}<!-- No arguments --></code>
<!-- 
GETNUMPLOTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|GetNumPlots}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMRESOURCES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|GetNumResources}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETNUMRESOURCESONLAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|GetNumResourcesOnLand}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETPLOT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetPlot}}<b>(</b>'''int''' x, '''int''' y = nil<b>)</b></code>
<!-- 
GETPLOTBYINDEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetPlotByIndex}}<b>(</b>{{Type5|PlotID}} index<b>)</b></code>
<!-- 
GETPLOTXY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetPlotXY}}<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset<b>)</b></code>
<!-- 
GETRANDOMRESOURCEQUANTITY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|Map|GetRandomResourceQuantity}}<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>
<!-- 
GETSEALEVEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Map|GetSeaLevel}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETWORLDSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|GetWorldSize}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==I==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ISPLOT
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|IsPlot}}<!-- No arguments --></code>
<!-- 
ISWRAPX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|IsWrapX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISWRAPY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|Map|IsWrapY}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==M==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
MAXPLOTDISTANCE
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|MaxPlotDistance}}<!-- No arguments --></code>
|}

==P==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
PLOTDIRECTION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Map|PlotDirection}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
PLOTDISTANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|PlotDistance}}<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset<b>)</b></code>
<!-- 
PLOTXYWITHRANGECHECK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Plot}}</code>
|width="100%" |<code>{{FuncLabel5|Map|PlotXYWithRangeCheck}}<b>(</b>'''int''' x, '''int''' y, '''int''' xOffset, '''int''' yOffset, '''int''' maxRange<b>)</b></code>
|}

==R==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
RAND
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Map|Rand}}<b>(</b>'''int''' maxValues, '''string''' logEntry<b>)</b></code>
<!-- 
RECALCULATEAREAS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|Map|RecalculateAreas}}<b>(</b><!-- No arguments --><b>)</b></code>
|}

==U==
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
UPDATEDEFERREDFOG
-->
|-
{{FuncInfos5|yesNeverUsed|yesNeverUsed|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|Map|UpdateDeferredFog}}<!-- No arguments --></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Map]]
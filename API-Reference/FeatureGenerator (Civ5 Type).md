{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This object is defined in the following Lua source file: ''FeatureGenerator.lua''.
:To import it, use: <code>include("FeatureGenerator")</code>}}


=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>FeatureGenerator.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CREATE
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|Create}}<b>(</b>'''table''' args<b>)</b></code>
|}


=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of FeatureGenerator.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
__INITFEATURETYPES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|__initFeatureTypes}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
__INITFRACTALS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|__initFractals}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDATOLLS
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddAtolls}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ADDFEATURES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddFeatures}}<b>(</b>'''int''' allow_mountains_on_coast<b>)</b></code>
<!-- 
ADDFEATURESATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddFeaturesAtPlot}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
<!-- 
ADDFORESTSATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddForestsAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDICEATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddIceAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDJUNGLESATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddJunglesAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDMARSHATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddMarshAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADDOASISATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AddOasisAtPlot}}<b>(</b>{{Type5|Plot}} plot, '''int''' x, '''int''' y, '''int''' lat<b>)</b></code>
<!-- 
ADJUSTTERRAINTYPES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|AdjustTerrainTypes}}<!-- No arguments --></code>
<!-- 
GETLATITUDEATPLOT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|FeatureGenerator|GetLatitudeAtPlot}}<b>(</b>'''int''' x, '''int''' y<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|FeatureGenerator]]
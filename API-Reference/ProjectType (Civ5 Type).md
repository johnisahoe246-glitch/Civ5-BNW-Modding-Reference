{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ProjectType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ProjectType</code> corresponds to the ''ID'' column of the {{Table5|Projects|CIV5Projects}} XML table.
}}


= XML: the Projects table =
Here are the ''ID'' and ''Type'' columns found in this table.
<code>
{|
|-
!align="left" |ID
!
!align="left" |Type
|-
|align="right"|0
|
|PROJECT_MANHATTAN_PROJECT
|-
|align="right"|1
|
|PROJECT_APOLLO_PROGRAM
|-
|align="right"|2
|
|PROJECT_SS_COCKPIT
|-
|align="right"|3
|
|PROJECT_SS_STASIS_CHAMBER
|-
|align="right"|4
|
|PROJECT_SS_ENGINE
|-
|align="right"|5
|
|PROJECT_SS_BOOSTER
|-
|align="right"|6
|
|PROJECT_UTOPIA_PROJECT
|}</code>


= Examples =
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Projects.PROJECT_MANHATTAN_PROJECT.ID
local id = GameInfo["Projects"].["PROJECT_MANHATTAN_PROJECT"].ID
local id = GameInfo.Projects{Type="PROJECT_MANHATTAN_PROJECT"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Cost'' column. Those examples will return and assign the value 750.
<syntaxhighlight lang="lua" class="civ5-example">
local cost = GameInfo.Projects[0].Cost
local cost = GameInfo["Projects"][0]["Cost"]
local cost = GameInfo.Projects{ID=0}().Cost
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
GETHELPTEXTFORPROJECT
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Func5|GetHelpTextForProject}}<b>(</b>{{Type5|ProjectType}} project, '''bool''' includeRequirementsInfo<b>)</b></code>
<!-- 
CANCREATE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|CanCreate}}<b>(</b>{{Type5|ProjectType}} project, '''int''' continue, '''int''' testVisible<b>)</b></code>
<!-- 
CHOOSEPRODUCTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ChooseProduction}}<b>(</b>{{Type5|UnitType}} trainUnit, {{Type5|BuildingType}} constructBuilding, {{Type5|ProjectType}} createProject, '''bool''' finish, '''bool''' front<b>)</b></code>
<!-- 
GETFIRSTPROJECTORDER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetFirstProjectOrder}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
GETPRODUCTIONPROJECT
-->
|-
|align="right" width="200" |<code>{{Type5|ProjectType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProductionProject}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETPROJECTPRODUCTIONMODIFIER
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProjectProductionModifier}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
GETPROJECTPRODUCTIONTURNSLEFT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProjectProductionTurnsLeft}}<b>(</b>{{Type5|ProjectType}} project, '''int''' num<b>)</b></code>
<!-- 
GETPROJECTPURCHASECOST
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetProjectPurchaseCost}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
CITYPURCHASEBUILDING
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseBuilding}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEPROJECT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseProject}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
CITYPURCHASEUNIT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|CityPurchaseUnit}}<b>(</b>{{Type5|City}} city, {{Type5|UnitType}} unitType, '''int''' buildingType, {{Type5|ProjectType}} projectTypes<b>)</b></code>
<!-- 
GETPROJECTCREATEDCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetProjectCreatedCount}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
ISPROJECTMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|IsProjectMaxedOut}}<b>(</b>{{Type5|ProjectType}} index, '''int''' extra<b>)</b></code>
<!-- 
CANCREATE
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanCreate}}<b>(</b>{{Type5|ProjectType}} project, '''bool''' continue, '''bool''' testVisible<b>)</b></code>
<!-- 
GETPROJECTPRODUCTIONNEEDED
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetProjectProductionNeeded}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
ISPRODUCTIONMAXEDPROJECT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsProductionMaxedProject}}<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>
<!-- 
CHANGEPROJECTCOUNT
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|ChangeProjectCount}}<b>(</b>{{Type5|ProjectType}} index, '''int''' change<b>)</b></code>
<!-- 
GETPROJECTARTTYPE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetProjectArtType}}<b>(</b>{{Type5|ProjectType}} index, '''int''' number<b>)</b></code>
<!-- 
GETPROJECTCOUNT
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetProjectCount}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
GETPROJECTDEFAULTARTTYPE
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetProjectDefaultArtType}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
GETPROJECTMAKING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|GetProjectMaking}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
ISPROJECTANDARTMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsProjectAndArtMaxedOut}}<b>(</b>{{Type5|ProjectType}} index<b>)</b></code>
<!-- 
ISPROJECTMAXEDOUT
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|IsProjectMaxedOut}}<b>(</b>{{Type5|ProjectType}} index, '''int''' extra<b>)</b></code>
<!-- 
SETPROJECTARTTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|SetProjectArtType}}<b>(</b>{{Type5|ProjectType}} index, '''int''' number, '''int''' value<b>)</b></code>
<!-- 
SETPROJECTDEFAULTARTTYPE
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Team}}:{{Func5|Team|SetProjectDefaultArtType}}<b>(</b>{{Type5|ProjectType}} index, '''int''' value<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ProjectType]]
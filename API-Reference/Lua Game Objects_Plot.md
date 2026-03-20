Plot objects represent a single instance of CvPlot.

=Member Methods=

==AddFeatureDummyModel==
''<summary>''

'''Usage'''

void plot:AddFeatureDummyModel(string dummyTag, string modelTag);

'''Parameters'''

:dummyTag
::No Description Available
:modelTag
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==Area==
''<summary>''

'''Usage'''

plot:Area();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==At==
''<summary>''

'''Usage'''

boolean plot:At(int iX, int iY);

'''Parameters'''

:iX
::No Description Available
:iY
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CalculateBestNatureYield==
''<summary>''

'''Usage'''

int plot:CalculateBestNatureYield([[YieldTypes]] eIndex, [[TeamTypes]] eTeam);

'''Parameters'''

:eIndex
::No Description Available
:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CalculateImprovementYieldChange==
''<summary>''

'''Usage'''

int plot:CalculateImprovementYieldChange([[ImprovementTypes]] eImprovement, [[YieldTypes]] eYield, [[PlayerTypes]] ePlayer, boolean bOptimal, [[RouteTypes]] eAssumeThisRoute);

'''Parameters'''

:eImprovement
::No Description Available
:eYield
::No Description Available
:ePlayer
::No Description Available
:bOptimal
::No Description Available
:eAssumeThisRoute
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CalculateNatureYield==
''<summary>''

'''Usage'''

int plot:CalculateNatureYield([[YieldTypes]] eIndex, [[TeamTypes]] eTeam, boolean bIgnoreFeature = false);

'''Parameters'''

:eIndex
::No Description Available
:eTeam
::No Description Available
:bIgnoreFeature
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CalculateTotalBestNatureYield==
''<summary>''

'''Usage'''

int plot:CalculateTotalBestNatureYield([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CalculateYield==
''<summary>''

'''Usage'''

int plot:CalculateYield([[YieldTypes]] eIndex, boolean bDisplay);

'''Parameters'''

:eIndex
::No Description Available
:bDisplay
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanBuild==
''<summary>''

'''Usage'''

boolean plot:CanBuild([[BuildTypes]] eBuild, [[PlayerTypes]] ePlayer, boolean bTestVisible);

'''Parameters'''

:eBuild
::No Description Available
:ePlayer
::No Description Available
:bTestVisible
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanHaveFeature==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanHaveImprovement==
''<summary>''

'''Usage'''

boolean plot:CanHaveImprovement([[ImprovementTypes]] eImprovement, [[TeamTypes]] eTeam, boolean bPotential);

'''Parameters'''

:eImprovement
::No Description Available
:eTeam
::No Description Available
:bPotential
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanHaveResource==
''<summary>''

'''Usage'''

boolean plot:CanHaveResource([[ResourceTypes]] eResource, boolean bIgnoreLatitude);

'''Parameters'''

:eResource
::No Description Available
:bIgnoreLatitude
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CanSeePlot==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeBuildProgress==
''<summary>''

'''Usage'''

boolean plot:ChangeBuildProgress([[BuildTypes]] eBuild, int iChange, [[TeamTypes]] eTeam);

'''Parameters'''

:eBuild
::No Description Available
:iChange
::No Description Available
:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeCulture==
Alters the culture 'yield' of the plot. This gives the tile a culture yield like that of a tile with a monument.

'''Usage'''

void plot:ChangeCulture(int iChange);

'''Parameters'''

:iChange
::The amount to change the tile's culture value by

'''Example'''

<pre>
No Example Available
</pre>

==ChangeExtraMovePathCost==
''<summary>''

'''Usage'''

void plot:ChangeExtraMovePathCost(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeImprovementDuration==
''<summary>''

'''Usage'''

void plot:ChangeImprovementDuration(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeInvisibleVisibilityCount==
''<summary>''

'''Usage'''

void plot:ChangeInvisibleVisibilityCount([[TeamTypes]] eTeam, [[InvisibleTypes]] eInvisible, int iChange);

'''Parameters'''

:eTeam
::No Description Available
:eInvisible
::No Description Available
:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeNumResource==
''<summary>''

'''Usage'''

void plot:ChangeNumResource(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeOwnershipDuration==
''<summary>''

'''Usage'''

void plot:ChangeOwnershipDuration(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeUpgradeProgress==
''<summary>''

'''Usage'''

void plot:ChangeUpgradeProgress(int iChange);

'''Parameters'''

:iChange
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ChangeVisibilityCount==
''<summary>''

'''Usage'''

void plot:ChangeVisibilityCount([[TeamTypes]] eTeam, int iChange, [[InvisibleTypes]] eSeeInvisibleType, boolean bInformExplorationTracking, boolean bAlwaysSeeInvisible);

'''Parameters'''

:eTeam
::No Description Available
:iChange
::No Description Available
:eSeeInvisibleType
::No Description Available
:bInformExplorationTracking
::No Description Available
:bAlwaysSeeInvisible
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==CountNumAirUnits==
''<summary>''

'''Usage'''

int plot:CountNumAirUnits([[TeamTypes]] ePlayer);

'''Parameters'''

:ePlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==DefenseModifier==
''<summary>''

'''Usage'''

int plot:DefenseModifier([[TeamTypes]] iDefendTeam, boolean bIgnoreBuilding, boolean bHelp);

'''Parameters'''

:iDefendTeam
::No Description Available
:bIgnoreBuilding
::No Description Available
:bHelp
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==Erase==
''<summary>''

'''Usage'''

void plot:Erase();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetArea==
''<summary>''

'''Usage'''

int plot:GetArea();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBestDefender==
''<summary>''

'''Usage'''

plot:GetBestDefender([[PlayerTypes]] eOwner, [[PlayerTypes]] eAttackingPlayer, [[Lua Game Objects/Unit|<Unit>]] pAttacker, boolean bTestAtWar, boolean bTestPotentialEnemy, boolean bTestCanMove);

'''Parameters'''

:eOwner
::No Description Available
:eAttackingPlayer
::No Description Available
:pAttacker
::No Description Available
:bTestAtWar
::No Description Available
:bTestPotentialEnemy
::No Description Available
:bTestCanMove
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBuildProgress==
''<summary>''

'''Usage'''

int plot:GetBuildProgress([[BuildTypes]] eBuild);

'''Parameters'''

:eBuild
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBuildTime==
''<summary>''

'''Usage'''

int plot:GetBuildTime([[BuildTypes]] eBuild);

'''Parameters'''

:eBuild
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBuildTurnsLeft==
''<summary>''

'''Usage'''

int plot:GetBuildTurnsLeft([[BuildTypes]] eBuild, int iNowExtra, int iThenExtra);

'''Parameters'''

:eBuild
::No Description Available
:iNowExtra
::No Description Available
:iThenExtra
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetBuildTurnsTotal==
''<summary>''

'''Usage'''

int plot:GetBuildTurnsTotal([[BuildTypes]] eBuild);

'''Parameters'''

:eBuild
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetCityRadiusCount==
''<summary>''

'''Usage'''

int plot:GetCityRadiusCount();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetContinentArtType==
''Determines continent for plot type.''

'''Usage'''

plot:GetContinentArtType()

'''Parameters'''

:
::No parameters.

''' Returns'''

Returns number 0=Ocean, 1=America, 2=Asia, 3=Africa, 4=Europa

'''Example'''

<pre>
local plot = Map.GetPlot(x, y);
if (plot:GetContinentArtType() == 1) then
print("America");
</pre>

==GetCulture==
Determines the amount of culture yielded by working the plot.

'''Usage'''

int plot:GetCulture();

'''Parameters'''

None

''' Returns'''

The amount of culture yielded by working the plot.

'''Example'''

<pre>
No Example Available
</pre>

==GetExtraMovePathCost==
''<summary>''

'''Usage'''

int plot:GetExtraMovePathCost();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetFeatureProduction==
''<summary>''

'''Usage'''

int plot:GetFeatureProduction([[BuildTypes]] eBuild, [[TeamTypes]] eTeam, [[Lua Game Objects/City|<City>]] ppCity);

'''Parameters'''

:eBuild
::No Description Available
:eTeam
::No Description Available
:ppCity
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetFeatureType==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetFeatureVariety==
''<summary>''

'''Usage'''

int plot:GetFeatureVariety();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetFoundValue==
''<summary>''

'''Usage'''

int plot:GetFoundValue([[PlayerTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetImprovementDuration==
''<summary>''

'''Usage'''

int plot:GetImprovementDuration();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetImprovementType==
''<summary>''

'''Usage'''

[[ImprovementTypes]] plot:GetImprovementType();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetInlandCorner==
''<summary>''

'''Usage'''

plot plot:GetInlandCorner();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetInvisibleVisibilityCount==
''<summary>''

'''Usage'''

int plot:GetInvisibleVisibilityCount([[TeamTypes]] eTeam, [[InvisibleTypes]] eInvisible);

'''Parameters'''

:eTeam
::No Description Available
:eInvisible
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetLatitude==
''<summary>''

'''Usage'''

int plot:GetLatitude();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNearestLandArea==
''<summary>''

'''Usage'''

int plot:GetNearestLandArea();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNearestLandPlot==
''<summary>''

'''Usage'''

plot:GetNearestLandPlot();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNonObsoleteResourceType==
''<summary>''

'''Usage'''

[[ResourceTypes]] plot:GetNonObsoleteResourceType([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumDefenders==
''<summary>''

'''Usage'''

int plot:GetNumDefenders([[PlayerTypes]] ePlayer);

'''Parameters'''

:ePlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumFriendlyUnitsOfType==
''<summary>''

'''Usage'''

int plot:GetNumFriendlyUnitsOfType([[Lua Game Objects/Unit|<Unit>]] pUnit);

'''Parameters'''

:pUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumResource==
''<summary>''

'''Usage'''

int plot:GetNumResource();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumUnits==
''<summary>''

'''Usage'''

int plot:GetNumUnits();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumVisibleEnemyDefenders==
''<summary>''

'''Usage'''

int plot:GetNumVisibleEnemyDefenders([[Lua Game Objects/Unit|<Unit>]] pUnit);

'''Parameters'''

:pUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetNumVisiblePotentialEnemyDefenders==
''<summary>''

'''Usage'''

int plot:GetNumVisiblePotentialEnemyDefenders([[Lua Game Objects/Unit|<Unit>]] pUnit);

'''Parameters'''

:pUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetOwner==
''<summary>''

'''Usage'''

[[PlayerTypes]] plot:GetOwner();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetOwnershipDuration==
''<summary>''

'''Usage'''

int plot:GetOwnershipDuration();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPlayerCityRadiusCount==
''<summary>''

'''Usage'''

int plot:GetPlayerCityRadiusCount([[PlayerTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPlotCity==
''<summary>''

'''Usage'''

plot:GetPlotCity();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetPlotType==
''<summary>''

'''Usage'''

[[PlotTypes]] plot:GetPlotType();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetReconCount==
''<summary>''

'''Usage'''

int plot:GetReconCount();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetResourceType==
''<summary>''

'''Usage'''

[[ResourceTypes]] plot:GetResourceType([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRevealedImprovementType==
''<summary>''

'''Usage'''

[[ImprovementTypes]] plot:GetRevealedImprovementType([[TeamTypes]] eTeam, boolean bDebug);

'''Parameters'''

:eTeam
::No Description Available
:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRevealedOwner==
''<summary>''

'''Usage'''

[[PlayerTypes]] plot:GetRevealedOwner([[TeamTypes]] eTeam, boolean bDebug);

'''Parameters'''

:eTeam
::No Description Available
:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRevealedRouteType==
''<summary>''

'''Usage'''

[[RouteTypes]] plot:GetRevealedRouteType([[TeamTypes]] eTeam, boolean bDebug);

'''Parameters'''

:eTeam
::No Description Available
:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRevealedTeam==
''<summary>''

'''Usage'''

[[TeamTypes]] plot:GetRevealedTeam([[TeamTypes]] eTeam, boolean bDebug);

'''Parameters'''

:eTeam
::No Description Available
:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRiverCrossingCount==
''<summary>''

'''Usage'''

int plot:GetRiverCrossingCount();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRiverEFlowDirection==
''<summary>''

'''Usage'''

[[FlowDirectionTypes]] plot:GetRiverEFlowDirection();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRiverSEFlowDirection==
''<summary>''

'''Usage'''

[[FlowDirectionTypes]] plot:GetRiverSEFlowDirection();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRiverSWFlowDirection==
''<summary>''

'''Usage'''

[[FlowDirectionTypes]] plot:GetRiverSWFlowDirection();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetRouteType==
''<summary>''

'''Usage'''

[[RouteTypes]] plot:GetRouteType();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetScriptData==
''<summary>''

'''Usage'''

string plot:GetScriptData();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetSelectedUnit==
''<summary>''

'''Usage'''

plot:GetSelectedUnit();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTeam==
''<summary>''

'''Usage'''

int plot:GetTeam();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetTerrainType==
''Use to retrieve the type of terrain on a given plot.  <br>Use [[Lua_Game_Objects/Plot#SetTerrainType|plot:SetTerrainType]] to change a terrain type.''

'''Usage'''

plot:GetTerrainType();

'''Parameters'''

:
::No Description Available

''' Returns'''

[[TerrainTypes]]

'''Example'''

<pre>
No Example Available
</pre>

==GetUnit==
''<summary>''

'''Usage'''

plot:GetUnit(int iIndex);

'''Parameters'''

:iIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetUnitPower==
''<summary>''

'''Usage'''

int plot:GetUnitPower([[PlayerTypes]] eOwner);

'''Parameters'''

:eOwner
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetUpgradeProgress==
''<summary>''

'''Usage'''

int plot:GetUpgradeProgress();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetUpgradeTimeLeft==
''<summary>''

'''Usage'''

int plot:GetUpgradeTimeLeft([[ImprovementTypes]] eImprovement, [[PlayerTypes]] ePlayer);

'''Parameters'''

:eImprovement
::No Description Available
:ePlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetVisibilityCount==
''<summary>''

'''Usage'''

int plot:GetVisibilityCount([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetWorkingCity==
''<summary>''

'''Usage'''

plot:GetWorkingCity();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetWorkingCityOverride==
''<summary>''

'''Usage'''

plot:GetWorkingCityOverride();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetX==
''<summary>''

'''Usage'''

int plot:GetX();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetY==
''<summary>''

'''Usage'''

int plot:GetY();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetYield==
''<summary>''

'''Usage'''

int plot:GetYield([[YieldTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==GetYieldWithBuild==
''<summary>''

'''Usage'''

boolean plot:GetYieldWithBuild();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==HasBarbarianCamp==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==HasYield==
''<summary>''

'''Usage'''

boolean plot:HasYield();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsActiveVisible==
''<summary>''

'''Usage'''

boolean plot:IsActiveVisible(boolean bDebug);

'''Parameters'''

:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentNonrevealed==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentNonrevealed([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentNonvisible==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentNonvisible([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentOwned==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentOwned();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentPlayer==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentPlayer([[PlayerTypes]] ePlayer, boolean bLandOnly);

'''Parameters'''

:ePlayer
::No Description Available
:bLandOnly
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentRevealed==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentRevealed([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentTeam==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentTeam([[TeamTypes]] eTeam, boolean bLandOnly);

'''Parameters'''

:eTeam
::No Description Available
:bLandOnly
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentToArea==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentToArea([[Lua Game Objects/Area|<Area>]] pArea);

'''Parameters'''

:pArea
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentToLand==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentToLand();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentToShallowWater==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentToShallowWater();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsAdjacentVisible==
''<summary>''

'''Usage'''

boolean plot:IsAdjacentVisible([[TeamTypes]] eTeam, boolean bDebug);

'''Parameters'''

:eTeam
::No Description Available
:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsBarbarian==
''<summary>''

'''Usage'''

boolean plot:IsBarbarian();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsBeingWorked==
''<summary>''

'''Usage'''

boolean plot:IsBeingWorked();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsBestAdjacentFound==
''<summary>''

'''Usage'''

boolean plot:IsBestAdjacentFound([[PlayerTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsBuildRemovesFeature==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsCity==
''<summary>''

'''Usage'''

boolean plot:IsCity();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsCityRadius==
''<summary>''

'''Usage'''

int plot:IsCityRadius();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsCoastalLand==
''<summary>''

'''Usage'''

boolean plot:IsCoastalLand();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsEnemyCity==
''<summary>''

'''Usage'''

boolean plot:IsEnemyCity([[Lua Game Objects/Unit|<Unit>]] pUnit);

'''Parameters'''

:pUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsFighting==
''<summary>''

'''Usage'''

boolean plot:IsFighting();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsFlatlands==
''<summary>''

'''Usage'''

boolean plot:IsFlatlands();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsFreshWater==
''<summary>''

'''Usage'''

boolean plot:IsFreshWater();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsFriendlyCity==
''<summary>''

'''Usage'''

boolean plot:IsFriendlyCity([[Lua Game Objects/Unit|<Unit>]] pUnit, boolean bCheckImprovement);

'''Parameters'''

:pUnit
::No Description Available
:bCheckImprovement
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsFriendlyTerritory==
''<summary>''

'''Usage'''

boolean plot:IsFriendlyTerritory([[PlayerTypes]] ePlayer);

'''Parameters'''

:ePlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsGoody==
''<summary>''

'''Usage'''

boolean plot:IsGoody();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsHills==
''<summary>''

'''Usage'''

boolean plot:IsHills();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsImpassable==
''<summary>''

'''Usage'''

boolean plot:IsImpassable();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsImprovementPillaged==
''<summary>''

'''Usage'''

boolean plot:IsImprovementPillaged();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsInvisibleVisible==
''<summary>''

'''Usage'''

boolean plot:IsInvisibleVisible([[TeamTypes]] eTeam, [[InvisibleTypes]] eInvisible);

'''Parameters'''

:eTeam
::No Description Available
:eInvisible
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsLake==
''<summary>''

'''Usage'''

boolean plot:IsLake();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsMountain==
''<summary>''

'''Usage'''

boolean plot:IsMountain();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsNEOfRiver==
''<summary>''

'''Usage'''

boolean plot:IsNEOfRiver();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsNone==
''<summary>''

'''Usage'''

boolean plot:IsNone();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsNWOfRiver==
''<summary>''

'''Usage'''

boolean plot:IsNWOfRiver();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsOpenGround==
''<summary>''

'''Usage'''

boolean plot:IsOpenGround();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsOwned==
''<summary>''

'''Usage'''

boolean plot:IsOwned();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsOwnershipScore==
''<summary>''

'''Usage'''

boolean plot:IsOwnershipScore();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsPlayerCityRadius==
''<summary>''

'''Usage'''

boolean plot:IsPlayerCityRadius([[PlayerTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsPotentialCityWork==
''<summary>''

'''Usage'''

boolean plot:IsPotentialCityWork();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsPotentialCityWorkForArea==
''<summary>''

'''Usage'''

boolean plot:IsPotentialCityWorkForArea([[Lua Game Objects/Area|<Area>]] pArea);

'''Parameters'''

:pArea
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsResourceConnectedByImprovement==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRevealed==
''<summary>''

'''Usage'''

boolean plot:IsRevealed([[TeamTypes]] eTeam, boolean bDebug);

'''Parameters'''

:eTeam
::No Description Available
:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRevealedBarbarian==
''<summary>''

'''Usage'''

boolean plot:IsRevealedBarbarian();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRevealedGoody==
''<summary>''

'''Usage'''

boolean plot:IsRevealedGoody([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRiver==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRiverConnection==
''<summary>''

'''Usage'''

boolean plot:IsRiverConnection([[DirectionTypes]] eDirection);

'''Parameters'''

:eDirection
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRiverCrossing==
''<summary>''

'''Usage'''

boolean plot:IsRiverCrossing([[DirectionTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRiverCrossingFlowClockwise==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRiverCrossingToPlot==
''<summary>''

'''Usage'''

boolean plot:IsRiverCrossingToPlot([[DirectionTypes]] eIndex);

'''Parameters'''

:eIndex
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRiverSide==
''<summary>''

'''Usage'''

boolean plot:IsRiverSide();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRoughGround==
''<summary>''

'''Usage'''

boolean plot:IsRoughGround();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRoute==
''<summary>''

'''Usage'''

boolean plot:IsRoute();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsRoutePillaged==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsStartingPlot==
''<summary>''

'''Usage'''

boolean plot:IsStartingPlot();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsTradeRoute==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsUnit==
''<summary>''

'''Usage'''

boolean plot:IsUnit();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsValidDomainForAction==
''<summary>''

'''Usage'''

boolean plot:IsValidDomainForAction([[Lua Game Objects/Unit|<Unit>]] pUnit);

'''Parameters'''

:pUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsValidDomainForLocation==
''<summary>''

'''Usage'''

boolean plot:IsValidDomainForLocation([[Lua Game Objects/Unit|<Unit>]] pUnit);

'''Parameters'''

:pUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsVisible==
''<summary>''

'''Usage'''

boolean plot:IsVisible([[TeamTypes]] eTeam, boolean bDebug);

'''Parameters'''

:eTeam
::No Description Available
:bDebug
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsVisibleEnemyDefender==
''<summary>''

'''Usage'''

boolean plot:IsVisibleEnemyDefender([[Lua Game Objects/Unit|<Unit>]] pUnit);

'''Parameters'''

:pUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsVisibleEnemyUnit==
''<summary>''

'''Usage'''

boolean plot:IsVisibleEnemyUnit([[PlayerTypes]] ePlayer);

'''Parameters'''

:ePlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsVisibleOtherUnit==
''<summary>''

'''Usage'''

boolean plot:IsVisibleOtherUnit([[PlayerTypes]] ePlayer);

'''Parameters'''

:ePlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsVisibleToWatchingHuman==
''<summary>''

'''Usage'''

boolean plot:IsVisibleToWatchingHuman();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsWater==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsWithinTeamCityRadius==
''<summary>''

'''Usage'''

boolean plot:IsWithinTeamCityRadius([[TeamTypes]] eTeam, [[PlayerTypes]] eIgnorePlayer);

'''Parameters'''

:eTeam
::No Description Available
:eIgnorePlayer
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==IsWOfRiver==
''<summary>''

'''Usage'''

boolean plot:IsWOfRiver();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==MovementCost==
''<summary>''

'''Usage'''

int plot:MovementCost([[Lua Game Objects/Unit|<Unit>]] pUnit, [[Lua Game Objects/Plot|<Plot>]] pFromPlot);

'''Parameters'''

:pUnit
::No Description Available
:pFromPlot
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==NukeExplosion==
''<summary>''

'''Usage'''

void plot:NukeExplosion(int iRange, [[Lua Game Objects/Unit|<Unit>]] pNukeUnit);

'''Parameters'''

:iRange
::No Description Available
:pNukeUnit
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==PickFeatureDummyTag==
''<summary>''

'''Usage'''

string plot:PickFeatureDummyTag(int mouseX, int mouseY);

'''Parameters'''

:mouseX
::No Description Available
:mouseY
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==RemoveGoody==
''<summary>''

'''Usage'''

void plot:RemoveGoody();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ResetFeatureModel==
''<summary>''

'''Usage'''

void plot:ResetFeatureModel();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SeeFromLevel==
''<summary>''

'''Usage'''

int plot:SeeFromLevel([[TeamTypes]] eTeam);

'''Parameters'''

:eTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SeeThroughLevel==
''<summary>''

'''Usage'''

int plot:SeeThroughLevel();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetArea==
''<summary>''

'''Usage'''

int plot:SetArea();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetContinentArtType==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetFeatureDummyTexture==
''<summary>''

'''Usage'''

void plot:SetFeatureDummyTexture(string dummyTag, string textureTag);

'''Parameters'''

:dummyTag
::No Description Available
:textureTag
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetFeatureDummyVisibility==
''<summary>''

'''Usage'''

void plot:SetFeatureDummyVisibility(string dummyTag, boolean show);

'''Parameters'''

:dummyTag
::No Description Available
:show
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetFeatureType==
''<summary>''

'''Usage'''

plot:();

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetImprovementDuration==
''<summary>''

'''Usage'''

void plot:SetImprovementDuration(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetImprovementPillaged==
''<summary>''

'''Usage'''

void plot:SetImprovementType(boolean b);

'''Parameters'''

:b
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetImprovementType==
''<summary>''

'''Usage'''

void plot:SetImprovementType([[ImprovementTypes]] eNewValue);

'''Parameters'''

:eNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetNEOfRiver==
''<summary>''

'''Usage'''

void plot:SetNEOfRiver(boolean bNewValue, [[FlowDirectionTypes]] eRiverDir);

'''Parameters'''

:bNewValue
::No Description Available
:eRiverDir
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetNumResource==
''<summary>''

'''Usage'''

void plot:SetNumResource(int iNum);

'''Parameters'''

:iNum
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetNWOfRiver==
''<summary>''

'''Usage'''

void plot:SetNWOfRiver(boolean bNewValue, [[FlowDirectionTypes]] eRiverDir);

'''Parameters'''

:bNewValue
::No Description Available
:eRiverDir
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetOwner==
''<summary>''

'''Usage'''

void plot:SetOwner([[PlayerTypes]] eNewValue, int iAcquiringCityID, boolean bCheckUnits = true, boolean bUpdateResources = true);

'''Parameters'''

:eNewValue
::No Description Available
:iAcquiringCityID
::No Description Available
:bCheckUnits
::No Description Available
:bUpdateResources
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetOwnershipDuration==
''<summary>''

'''Usage'''

void plot:SetOwnershipDuration(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetPlotType==
''<summary>''

'''Usage'''

void plot:SetPlotType([[PlotTypes]] eNewValue, boolean bRecalculate, boolean bRebuildGraphics);

'''Parameters'''

:eNewValue
::No Description Available
:bRecalculate
::No Description Available
:bRebuildGraphics
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetResourceType==
''<summary>''

'''Usage'''

void plot:SetResourceType([[ResourceTypes]] eNewValue, int iNumResource);

'''Parameters'''

:eNewValue
::No Description Available
:iNumResource
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetRevealed==
''<summary>''

'''Usage'''

void plot:SetRevealed([[TeamTypes]] eTeam, boolean bNewValue, boolean bTerrainOnly, [[TeamTypes]] eFromTeam);

'''Parameters'''

:eTeam
::No Description Available
:bNewValue
::No Description Available
:bTerrainOnly
::No Description Available
:eFromTeam
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetRouteType==
''<summary>''

'''Usage'''

void plot:SetRouteType([[RouteTypes]] eNewValue);

'''Parameters'''

:eNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetScriptData==
''<summary>''

'''Usage'''

void plot:SetScriptData(string szNewValue);

'''Parameters'''

:szNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetStartingPlot==
''<summary>''

'''Usage'''

void plot:SetStartingPlot(boolean bNewValue);

'''Parameters'''

:bNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetTerrainType==
''Use to set the terrain on a given plot.  <br>Graphics will refresh only after a save, exit to main menu and reload<br>Use with [[Lua_Game_Objects/Plot#GetTerrainType|plot:GetTerrainType]]''

'''Usage'''

plot:SetTerrainType([[TerrainTypes]] type);

'''Parameters'''

:
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetUpgradeProgress==
''<summary>''

'''Usage'''

void plot:SetUpgradeProgress(int iNewValue);

'''Parameters'''

:iNewValue
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==SetWOfRiver==
''<summary>''

'''Usage'''

void plot:SetWOfRiver(boolean bNewValue, [[FlowDirectionTypes]] eRiverDir);

'''Parameters'''

:bNewValue
::No Description Available
:eRiverDir
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==ShareAdjacentArea==
''<summary>''

'''Usage'''

boolean plot:ShareAdjacentArea([[Lua Game Objects/Plot|<Plot>]] pPlot);

'''Parameters'''

:pPlot
::No Description Available

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==UpdateFog==
''<summary>''

'''Usage'''

void plot:UpdateFog();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==UpdateVisibility==
''<summary>''

'''Usage'''

void plot:UpdateVisibility();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==WaterArea==
''<summary>''

'''Usage'''

plot:WaterArea();

'''Parameters'''

None

''' Returns'''

No Description Available.

'''Example'''

<pre>
No Example Available
</pre>

==See also==
* Other [[Lua Game Objects]]
* Querying database data over [[Lua Game Objects/GameInfo|GameInfo]]
* [[Gameplay Database Overview#Lua_Exposures|Gameplay Database Overview]]
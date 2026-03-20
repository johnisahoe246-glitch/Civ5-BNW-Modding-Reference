The '''CvCity''' file controls everything that occurs in each city in the game. Everything from Religion spread, Meltdowns, and city growth are controlled here.

The SDK files are written in the C++ programming language.  They can be edited in a text editor such as notepad or in a programming editor like Microsoft's Visual Studio.

<font color=red>This page is missing information. Do not remove this notice until it is complete.</font>

==Functions==

Below is a list of all the functions in the file. Each function has a quick description attached to it. Note that there are comments strewn throughout some of these files, direct from the developers in order to aid the potential modders. All these functions are in the class CvCity.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Function 
! style="background:#efefef;" | Parameters
! style="background:#efefef;" | Return Type 
! style="background:#efefef;" | Description
|-
!CvCity::CvCity()
|None
|Void
|Initializes and creates references for the arrays for each city ID
|-
!CvCity::~CvCity()
|None
|Void
|Clears the arrays of all data and size
|-
!CvCity::init()
|int iID, PlayerTypes eOwner, int iX, int iY, bool bBumpUnits, bool bUpdatePlotGroups
|Void
|Begins the initial city setup, finds the plot the city is located on, updates the city's culture, line of sight, destroys any features the city is built on top of, adds a road underneath the city, adds any initial free buildings, etc...
|-
!CvCity::uninit()
|None
|Void
|Clears all the arrays of size and data, for when the game is shutting down, or the city is destroyed.
|-
!CvCity::reset()
|int iID, PlayerTypes eOwner, int iX, int iY, bool bConstructorCall
|Void
|Initializes all variables and arrays to their default value (usually 0 or -1)
|-
!CvCity::setupGraphical()
|None
|Void
|Sets up the graphical display for the city
|-
!CvCity::kill
|bool bUpdatePlotGroups
|Void
|Destroys the city, called when the city is razed.
|-
!CvCity::doTurn()
|None
|Void
|Called each turn by CvGame. Does all of the standard actions a city experiences, growth, religion spread, Great People, Production... etc..
|-
!CvCity::isCitySelected()
|None
|Boolean
|returns true or false if a particular city is selected or not
|-
!CvCity::canBeSelected()
|None
|Boolean
|Called to see if the active team member can select the city in question or not. 
|-
!CvCity::updateSelectedCity()
|bool bTestProduction
|Void
|Updates the selected cities symbols and surrounding tiles.
|-
!CvCity::updateYield()
|None
|Void
|Loops through each city plot and calls the CvPlot::updateYield() function.
|-
!CvCity::updateVisibility()
|None
|Void
|Called at the start of the game and removes the fog of war and adds visibility for the city
|-
!CvCity::createGreatPeople()
|UnitTypes eGreatPersonUnit, bool bIncrementThreshold, bool bIncrementExperience
|Void
|Calls the CvPlayer::createGreatPeople function.
|-
!CvCity::doTask()
|TaskTypes eTask, int iData1, int iData2, bool bOption, bool bAlt, bool bShift, bool bCtrl
|Void
|Called when a player commands a city to do a task (like hurry production), and calls the function for the specific task that was called, or does nothing if it is given an invalid task type.
|-
!CvCity::chooseProduction()
|UnitTypes eTrainUnit, BuildingTypes eConstructBuilding, ProjectTypes eCreateProject, bool bFinish, bool bFront
|Void
|Creates the pop-up for the human player to choose the next construction project that the city will have, and fills it with the recommended unit, or recommended building, or the recommended project. This function is only used for the human player. 
|-
!CvCity::getCityPlotIndex()
|CvPlot* pPlot
|Int
|Returns the index number of the plot given.
|-
!CvCity::getCityIndexPlot()
|int iIndex
|CvPlot*
|Returns plot X,Y coordinates of the given index number.
|-
!CvCity::canWork()
|CvPlot* pPlot
|Boolean
|Given a plot, canWork() returns true or false if the city can work the plot.
|-
!CvCity::verifyWorkingPlot()
|int iIndex
|Void
|Ensures that the plot with the given index in the city is being worked is updated graphically and marked internally as being worked.
|-
!CvCity::verifyWorkingPlot()
|None
|Void
|Loops through all the city plots an calls verifyWorkingPlot() for each one.
|-
!CvCity::clearWorkingOverride()
|int iIndex
|Void
|Given a city plot index, clearWorkingOverride() overrides any previous settings and marks the plot as unworked.
|-
!CvCity::countNumImprovedPlots()
|ImprovementTypes eImprovement, bool bPotential
|Int
|Checks all the cities tiles for the given improvement type. If bPotential is true, it also counts possible sites for the given improvement.
|-
!CvCity::countNumWaterPlots()
|None
|Int
|Returns the number of the water tiles in the cities radius.
|-
!CvCity::countNumRiverPlots()
|None
|Int
|Returns the number of the tiles with a river on them in the cities radius.
|-
!CvCity::findPopulationRank()
|None
|Int
|Returns the rank of the city vs all other of the player's cities population. A Higher rank equates to a higher relative population.
|-
!CvCity::findBaseYieldRateRank()
|YieldTypes eYield
|Int
|Returns the rank of the city vs all other of the player's cities, for the given base yield type. A Higher rank equates to a higher relative yield.
|-
!CvCity::findYieldRateRank()
|YieldTypes eYield
|Int
|Returns the rank of the city vs all other of the player's cities, for the given yield type, after all yield modifiers have been applied (from civics, buildings, etc...). A Higher rank equates to a higher relative yield.
|-
!!CvCity::findCommerceRateRank()
|CommerceTypes eCommerce
|Int
|Returns the rank of the city vs all other of the player's cities, for the given commerce type. A Higher rank equates to a higher relative commerce.
|-
!CvCity::allUpgradesAvailable()
|UnitTypes eUnit, int iUpgradeCount
|UnitTypes
|Returns the unittype of the upgrade unit for the given unit, if any is available. If none are available, returns -1 (NO_UNIT).
|-
!CvCity::isWorldWondersMaxed()
|None
|Boolean
|Returns true if the city has exceeded the maximum limit for world wonders.
|-
!CvCity::isTeamWondersMaxed()
|None
|Boolean
|Returns true if the city has exceeded the maximum limit for team wonders.
|-
!CvCity::isNationalWondersMaxed()
|None
|Boolean
|Returns true if the city has exceeded the maximum limit for national wonders.
|-
!CvCity::isBuildingsMaxed()
|None
|Boolean
|Returns true if the city has exceeded the maximum limit for the # of buildings.
|-
!CvCity::getFoodTurnsLeft()
|None
|Int
|Get the number of turns left, until city will grow, according to current food left and current growth treshold
|}

{{Civ4_SDK_Files}}
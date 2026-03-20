''This page is a part of the [[Civ5 Modding Tutorials]].''

= Hard limits =
Limits you won't be able to circumvent.
* '''Audio'''
:A mod cannot add its own audio files
* '''3D leader scenes''' 
:They use a proprietary format. Although a paper has been published that explains how the algorithm works, the details of the implementation are unknown and as of August 2012 there is not tool to read or write them.
* '''Combat mechanics'''
:Since the pre-G&K patch the combat is no longer moddable.
* '''AI'''
:Most of it is processed on the C++ side and the API exposes almost no hooks to replace, trigger or prevent the standard behaviors. Now the diplomacy UI may be slightly modded though bonuses, and the fact that a mod can give orders to units opens a theoritical way to override the tactical and strategical UI although the daunting amount of work required and the involved CPU cost when comparing to Lua to C++ probably just makes this an illusion.
* '''Terrain modifications'''
:When they require an update of the 3D mesh (changing the TerrainType or the PlotType, and removing a feature), this one is not dynamically updated, the game needs to be reloaded. No terraforming mod.
* '''No more than 200 promotions'''
:Any promotion after that is added to every unit in the game. The base game with all DLC and expansion have about 165 promotions, so mods are restricted to less than 35 promotions in total. '''Will be removed in the 2012 Fall patch.'''
* '''No more than 22 major civilizations and 41 city states'''
:More hard-coded values.
* '''Espionage'''
:There is about no API to control it (no way to add/remove spies for example).
* '''Religious units'''
:There is no API to set a unit's religion.
* '''Civilizations without overrides'''
:A civilization that doesn't have at least two overrides (unique units/buildings) will not appear in the civilization selection screen.


= Soft limits =
Limits that can be overcame.
* '''Some assets cannot be deleted'''
:Deleting them causes the game to crash. Try to disable them instead.
* '''No more than one leader per civilization'''
:The Lua code for the setup screen only keeps the first leader for every civilization. You would need to use a modified version of the setup screen.


= Modularity problems =
Things that only one mod can do at the same time because it requires the full replacement of some resources. The community could theoretically issue solutions in some cases but in practice there is rarely a solution available.
* '''Units arts'''
:UnitMemberArtInfos and UnitArtInfos must be replaced altogether.
* '''UI'''
:Most of the UI mods need to replace some parts of the UI with their custom versions.
* '''Resources placement'''
:It requires the replacement of some of the AssignStartingPlots functions
* '''Natural wonders placement'''
:For the same reasons than resources.


[[Category:Civ5 Tutorials]]
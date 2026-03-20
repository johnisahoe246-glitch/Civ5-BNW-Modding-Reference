Over the years there have been several proposals from within the modding community to either expand Civilization III's source code or to create an independent game based on it. None of these ideas have yet come to fruition, although they have generated much discussion on the direction that we would like to take in such a game. This page is an overview of past attempts and a collection of ideas that have been proposed. It should serve as a guide for any future discussion to avoid repeating the same arguments and mistakes that have already been covered.

== Projects ==
===[http://forums.civfanatics.com/showthread.php?t=122220 Humanitas]===
Humanitas was a Civ-based game developed by Snoopy and jimmyh, announced in 2005 when it had already been in development for 2 years. It featured detailed map graphics and many new gameplay features, but no demo or code was ever released. Snoopy posted a list of [http://forums.civfanatics.com/showthread.php?t=122220 gameplay details] suggesting that the game was mature enough to be playable, though these may have been planned features. The project remained active at least through 2006.
===[http://forums.civfanatics.com/forumdisplay.php?f=441 IndieCiv]===
jimmyh, co-creator of Humanitas, began working on IndieCiv with a small team of beta testers in May 2011 after a [http://forums.civfanatics.com/showthread.php?t=421582 lengthy public discussion] on possibilities for an independent game. It is a Civ3 clone intended to evolve organically with new features. After a brief beta period, the project appears to have been abandoned in June 2011.
===[http://forums.civfanatics.com/forumdisplay.php?f=297 SSS/SGF]===
StrateGames Factory, originally known as [http://forums.civfanatics.com/showthread.php?t=59020 Steph's Strategic Simulation], is an ambitious turn-based 4X strategy platform/engine written in C# with XNA by Steph that has gone through a few phases of development since 2004. It currently offers graphical map engine and inheritance-based object editor. It is intended to be a powerful, flexible game system that allows for nearly unlimited customization from Civ-clone to something entirely different. The project has been inactive recently as Steph is working on his various other projects, but has not been abandoned.
===[http://freshmeat.net/projects/conquests Conquests]===
Conquests is an open-source clone in C++ by mdwh. From its project page on freshmeat.net:
<blockquote>Conquests is a turn-based 4X Civilization-like 3D strategy game. You can discover new technologies from the stone age to the space age, explore the world, and wage war on your opponents. It supports both Direct3D and OpenGL graphics, and can run in both 2D and 3D modes.</blockquote>
Conquests is an active project as of September 2011 but mdwh seems to be working alone with little community support.
===[http://forums.civfanatics.com/showthread.php?t=116293 Civilization Game Toolkit]===
This is an open-source Java application by jeyries that serves as a "scenario viewer": it loads scenario files and creates a somewhat interactive world map using Civ3's art files. He stated that his goal was to create an exact clone of Civ3 using Java. No progress on this project has been seen since jeyries posted the code in 2005.
=== [http://evolutiongame.angelfire.com/ Evolution] ===
Danny Rennó's EVOLUTION is a Civ3-based game written in C#, featuring the ancient world. It is under active development and an early demo version is available for download.

== Notable Discussion Threads ==
*[http://forums.civfanatics.com/forumdisplay.php?f=297 Steph's Workshop] forum for SGF discussion (limited access)
*[http://forums.civfanatics.com/forumdisplay.php?f=441 Project: Independent Civ Development] forum for IndieCiv discussion (limited access)
*[http://forums.civfanatics.com/showthread.php?t=421582 Independent Game Ideas]: jimmyh, May 2011. General discussion on the idea of an independent game and the direction it should take. Led to the establishment of IndieCiv.
*[http://forums.civfanatics.com/showthread.php?t=356726 What option for my game?] Steph, March 2010, about major design decisions for SGF
*[http://forums.civfanatics.com/showthread.php?t=309306 Possible new civilization game: make our own!] Steph, Feb 2009. Resumed work on SGF following the source code fall-through and led to much participation in establishing the direction of the project.
*[http://forums.civfanatics.com/showthread.php?t=272184 About That Source Code ...] Ozymandias, 2008. Serious campaign for the release of Civ3 source code and our proposals to make use of it
*[http://forums.civfanatics.com/showthread.php?t=59020 Steph's next great project announcement] Steph, July 2003. Origin of SSS.

== Proposed Features ==
'''Brief''' summaries of major proposed features should go here, including differences from Civ3, with links to applicable threads/posts if they generated a lot of discussion. Comments about how to best '''represent features on this page''' should be taken to this page's [http://modiki.civfanatics.com/index.php?title=Talk:Independent_Game_Ideas&action=edit Discussion page]. If a feature was controversial, please include '''proposals from both sides''' of the argument (for example, Civ3-compatible graphics vs a while new graphics engine).

'''This page is not for debates.''' Simply describe the concept, even if it conflicts with other proposals.
=== Scope & Direction ===
*The game should focus first on duplicating Civ3 features without bugs and numerical limits, then add new features. It should in effect be a Civ3 clone, with the possibility of more.
*The game should be redesigned from the ground up to be a Civ-like game, or a flexible engine that allows for a Civ-like game, but not seek specifically to duplicate Civ3 gameplay. Many suggested features are not compatible with a Civ3 clone.

=== Technical Considerations ===
=== Modding Considerations ===
*A powerful, flexible editor is provided that allows modders to make all necessary game changes without using any external applications.
*Alternatively, a scripting module and/or SDK allows programmers to further modify game behavior beyond the scope of the editor.
*Prerequisites are defined using arbitrary boolean expressions so that an item may require any combination of other items. For example, Tech A requires (Tech-B AND Tech-C) OR (Tech-D AND NOT Resource-E).

=== Basic Gameplay ===
=== General Graphics ===
==== Graphics Compatibility ====
*The game's graphics should be fully compatible with existing Civ3 formats. In other words, applicable Civ3 art files should be reused without modification.
*Alternatively, the game should seek to use Civ3-style graphics whenever possible, with the same perspective and resolution, but not limit itself to the existing format. Civ3 art files can be converted to new, more flexible file types such as PNG in RGB mode without changing the images themselves.

=== Map, Tiles, & Terrain ===
=== Units & Combat ===
=== Civilizations & Players ===
=== Techs & Eras ===
*Eras may be added or removed arbitrarily in the editor. Era-specific graphics are defined in the configuration, so there is no limit to the number of eras that may be used.
*Techs may be made (un)available to any civilization or player.
*Techs may be rendered obsolete by the discovery of another tech, such that a player must choose to research one or another branch of knowledge.

=== Cities & Buildings ===
=== Economics & Resources ===
=== Diplomacy, Espionage, & Victory ===
=== Events & Scripting ===
=== New Concepts ===

== See Also ==
*[http://forums.civfanatics.com/showthread.php?t=347039 Civ "expansion": more eras and evolutive civs!] by Steph
*[http://forums.civfanatics.com/showthread.php?t=369388 New idea for evolutive civ and updrade of units] by Steph
[[Category:Civilization 3]]
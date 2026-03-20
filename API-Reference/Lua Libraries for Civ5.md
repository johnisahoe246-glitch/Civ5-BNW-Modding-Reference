''This page is a part of the [[Lua and UI Reference (Civ5)|Lua and UI Reference]].''


= Improving modularity and mods compatibility =
Sometimes mods needs to modify the standard game files in order to achieve some features. Since only one mod can modify a given file a a time, this creates conflicts. Those libraries address those issues: all mods use the same file replacement and this one exposes a way to register new entries and such.
{| cellpadding="4"
|-
!Name
!Author
!Description
|-
|valign="top" |[http://forums.civfanatics.com/showthread.php?t=411186 Fully Modifyable Custom Notifications]
|valign="top" |''Sneaks''
|Provides a non-conflicting way for mods to add custom notifications.
|-
|valign="top" |[http://forums.civfanatics.com/showthread.php?p=11394279 Modular Diplo Corner]
|valign="top" |''Whoward69''
|Provides a non-conflicting way for mods to add entries to the diplo corner menu. While Civ5 now offers a similar functionality in standard, this mod still offers the benefit to prevent compatibility issues between updated and outdated mods.
|-
|valign="top" |[http://forums.civfanatics.com/showthread.php?t=458740 Modular Minimap Overlays]
|valign="top" |''Whoward69''
|Provides a non-conflicting way for mods to add entries to the minimap overlays menu.
|-
|valign="top" |[http://forums.civfanatics.com/showthread.php?t=459207 Modular Summary Bar]
|valign="top" |''Whoward69''
|Provides a non-conflicting way for mods to add entries to the topmost bar, near the turn number.
|}


= Other libraries =
{| cellpadding="4"
|-
!Name
!Author
!Description
|-
|[http://forums.civfanatics.com/showthread.php?t=474634 Border and Area Plot Iterators]
|''Whoward69''
|Provides iterators to enumerate plots in a given range and in different orders.
|-
|[http://forums.civfanatics.com/showthread.php?t=392958 SaveUtils] 
|''Whys''
|Wrappers around the SetScriptData methods (partially deprecated) for conveniency purpose and mods conflicts prevention. See also [[Persisting data (Civ5)]].
|-
|[http://forums.civfanatics.com/showthread.php?t=442249 TableSaverLoader] 
|''Pazyryk''
|Saves a Lua table into a custom data table. See also [[Persisting data (Civ5)]].
|}


[[Category:Civ5 API]]
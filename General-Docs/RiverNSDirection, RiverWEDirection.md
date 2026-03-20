'''RiverNSDirection'''= and '''RiverWEDirection'''= the direction that the water flows along the river. Valid values are 0=north, 1=east, 2=south, 3=west. These settings MUST be used in conjunction with [[IsNOfRiver,_isWOfRiver|isNOfRiver or isWOfRiver]]. EG:
 isNOfRiver
 RiverWEDirection=3
 # This will create a river on the bottom edge of the tile flowing from right to left.
 
 isWOfRiver
 RiverNSDirection=0
 # This will create a river on the right edge of the tile flowing from bottom to top.

{{Civ4_World_Builder}}
{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



= Purpose =
This object allows you to easily get a data row ID from its type. Example:
<syntaxhighlight lang="lua" class="civ5-example">
local settlerID = GameInfoTypes["UNIT_SETTLER"]
local settlerID = GameInfoTypes.UNIT_SETTLER
</syntaxhighlight>

This object '''does''' reflect the changes made by mods. It includes the type for your custom units, buildings, etc.


= Identifiers in the civ5 API =
Anytime you need to provide a reference to a data row somewhere in the API, you will need to provide its ID value. You could directly use numeric constants but this is hard to read and understand, and it is not robust since those identifiers can be modified by mods or future expansions. This is why it is better to use GameInfoTypes to make the conversion. Example:
<syntaxhighlight lang="lua" class="civ5-example">
-- GetUnitType returns the data row's ID, we compare it to the settler row's ID.
if (pUnit:GetUnitType() == GameInfoTypes.UNIT_SETTLER) then
-- This is equivalent to the following line, but this latter one is less clean and robust.
if (pUnit:GetUnitType() == 0) then
</syntaxhighlight>




{{Civ5 API Footer}}
[[Category:Civ5 Types|GameInfoTypes]]
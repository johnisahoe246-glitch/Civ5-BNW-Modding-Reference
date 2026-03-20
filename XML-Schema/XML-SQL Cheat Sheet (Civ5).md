''This page is a part of the [[Civ5 XML Reference]].''

= Things to remember =
* '''Booleans:''' SQLite does not have booleans, it uses integers. So do not use <code>true</code> or <code>false</code>, use <code>1</code> and <code>0</code>.


= Inserting rows =
=== XML ===
<div class="civ5-example"><syntaxhighlight lang="xml" style="left:40px;">
<GameData>
	<Colors>
            <!-- Inserts a new color -->
            <Row>
                <Type>COLOR_CUSTOM</Type>
                <Red>0.1</Red>
                <Green>0.1</Green>
                <Blue>0.1</Blue>
                <Alpha>0.45</Alpha>
            </Row>	
	</Colors>
<GameData>
</syntaxhighlight></div>

=== SQL ===
<div class="civ5-example"><syntaxhighlight lang="sql">
/* Inserts a new color */
INSERT INTO Colors (Type, Red, Green, Blue, Alpha)
VALUES ('COLOR_CUSTOM', 0.1, 0.1, 0.1, 0.45);
</syntaxhighlight></div>


= Deleting rows =
{{Warning}} See [http://forums.civfanatics.com/showthread.php?t=463429 Deleting data and issues, and how to avoid them] if you plan to delete rows and are not aware of the troubles that may arise.
=== XML ===
<div class="civ5-example"><syntaxhighlight lang="xml">
<GameData>
	<Colors>
            <!-- Deletes all colors named COLOR_CUSTOM (there is only one actually) -->
            <Delete Type="COLOR_CUSTOM" />
            <!-- You can specify as many conditions as you want -->
            <Delete R="1" G="1"/>
	</Colors>
<GameData>
</syntaxhighlight></div>

=== SQL ===
<div class="civ5-example"><syntaxhighlight lang="sql">
/* Deletes all colors named TYPE_CUSTOM whose red channel is equal to 1 */
DELETE FROM Colors
WHERE Type = 'COLOR_CUSTOM' AND Red = 1;
</syntaxhighlight></div>


= Updating rows =
=== XML ===
<div class="civ5-example"><syntaxhighlight lang="xml">
<GameData>
	<Colors>
            <!-- Changes the red channel for all colors named COLOR_CUSTOM (there is only one actually)
            <Update>
                <Where Type="COLOR_CUSTOM"/>
                <Set Red="1"/>
            </Update>
            <!-- You can specify as many conditions as you want and set as many properties as you want -->
            <Update>
                <Where Type="COLOR_CUSTOM" Red="0"/>
                <Set Red="1" Green="0"/>
            </Update>
            <!-- As always, formatting rules are relaxed, use what's the most convenient for you -->
            <Update>
                <Where>
                    <Type>COLOR_CUSTOM</Type>
                </Where>
                <Set>
                    <Red>1</Red>
                    <Green>1</Green>
                </Set>
            </Update>
        </Colors>
</GameData>
</syntaxhighlight></div>

=== SQL ===
<div class="civ5-example"><syntaxhighlight lang="sql">
/* Update all colors whose names are COLOR_CUSTOM and red channel is 0 */
UPDATE Colors
SET Red = 1, Green = 0
WHERE Type = 'COLOR_CUSTOM' AND Red = 0;

/* Makes everything brighter */
UPDATE Colors
SET Red = Red + 0.1, Green = Green + 0.1, Blue=Blue + 0.1;
</syntaxhighlight></div>


= New tables =
=== XML ===
<div class="civ5-example"><syntaxhighlight lang="xml">
<GameData>
    <Table Name="MyColors">
	<Column name="ID" type="integer" primarykey="true" autoincrement="true"/>
	<Column name="Type" type="text" notnull="true" unique="true"/>
    </Table>
</GameData>
</syntaxhighlight></div>

=== SQL ===
<div class="civ5-example"><syntaxhighlight lang="sql">
/* Create one new table with two columns */
CREATE TABLE MyColors( id INTEGER PRIMARY KEY AUTOINCREMENT, Type TEXT UNIQUE );
</syntaxhighlight></div>


= New columns =
=== SQL ===
<div class="civ5-example"><syntaxhighlight lang="sql">
/* Adds one Description column to Colors. */
ALTER TABLE Colors COLUMN 'Description' TEXT DEFAULT NULL;
</syntaxhighlight></div>


[[Category:Civ5 XML Files]]
[[Category:Civ5 Tutorials]]
This small tutorial is an attempt to bring some light into how you can actually use the provided string forms, genders and plurality. It is recommended to read [http://wiki.2kgames.com/civ5/index.php/Mods:AddingNewLanguage Adding New Language] and [http://wiki.2kgames.com/civ5/index.php/Mods:LocalizationSyntax Localization Syntax] first as this tutorial mostly focuses on details not available in the official documentation.

Information on this page is based on Civilization V version 1.0.2.21


==Transforms==

===:gender===

Gender transform allows you to select which text alongside the currently active gender is shown depending on what the gender is.

First here we have some sample data to look at:

<pre><Row Tag="TXT_KEY_SAMPLE">
    <Text>Form 1|Form 2|Form 3|Form 4</Text>
    <Gender>neuter:trait_one|masculine:trait_two|feminine:trait_three|mixed:trait_four</Gender>
</Row></pre>

neuter, masculine, feminine and mixed are hardcoded gender values and must be used. The second part values after : are called traits and you can call them anything you like. They can be left undefined, so you can do something like this as well:

<pre><Row Tag="TXT_KEY_TRAIT_GRACIOUS">
    <Text>Courtois|Courtoise</Text>
    <Gender>masculine|feminine</Gender>
</Row></pre>


A practical French sample:

<pre>{1:gender *:vowel?l'; masculine?le ; feminine?la ;}{1}</pre>

* '''le garçon''' ("garçon" is masculine)
* '''la fille''' ("fille" is feminine)
* '''l'arbre''' ("arbre" is masculine)
* '''l'église''' ("église" is feminine)

Or against TXT_KEY_SAMPLE:

* le Form 2
* la Form 3

Note that at this point the system knows which is the selected gender for {1} and thus the result depends on that. You can find information on how to select a specific gender manually further below in this article.


===:plural===

Allows you to define a plural form.

<pre><Row Tag="TXT_KEY_HORSE">
    <Text>hevonen|hevosta|hevoset|hevosista</Text>
    <Gender>neuter:nominative|neuter:elative|neuter:nominative|neuter:elative</Gender>
    <Plurality>1|1|2|2</Plurality>
</Row></pre>

The sample above is already a slightly complex case as the basic Finnish form for a "horse" is "hevonen" and "horses" would be "hevoset". However when dealing with numbers Finnish uses elative case when we are telling how many horses we have, which is unlike English.

====Plurality with just the number====

{1} = any number
{2} = TXT_KEY_HORSE

<pre>{1:plural 1?Yksi {2}; other?{1} {2 ^ 'neuter:elative'};}</pre>

Results:
* Yksi hevonen (one horse)
* 2 hevosta (two horses)
* 3 hevosta (three horses)

====Plurality with everything====

{1} = any number
{2} = TXT_KEY_HORSE

<pre>{1:plural 1?Yksi {2}; other?{1} {2 * {1} ^ 'neuter:elative'};}</pre>

Results:
* Yksi hevonen (one horse)
* 2 hevosista (two of the horses)
* 3 hevosista (three of the horses)


===TODO===
* :textkey
* :upper
* :lower
* :title
* :percent
* :number
* :roman
* :spellout


==Forms, gender and plurality==

Sample data:

<pre><Row Tag="TXT_KEY_SAMPLE">
    <Text>Form 1|Form 2|Form 3|Form 4</Text>
    <Gender>neuter:trait_one|masculine:trait_two|feminine:trait_three|mixed:trait_four</Gender>
    <Plurality>1|1|1|2</Plurality>
</Row></pre>

In the following examples '''there must be no lookup @ character''' with any form, gender or plural selection.

===Selecting a form===

You can select a specific form by using brackets.

<pre><Text>This is my {1_Sample[2]}</Text></pre>

Result: "This is my Form 2"


===Selecting a gender===

<pre><Text>This is my {1_Sample ^ 'feminine:trait_three'}</Text></pre>

Result: "This is my Form 3"


===Selecting a plural===

2_Num = 2

<pre><Text>This is my {1_Sample * 2_Num}</Text></pre>

Result: "This is my Form 4"


===Transforms with forms, gender or plural===

You cannot mix a form, gender or plural selector with a transform. '''Transform always applies to the first form available'''. If there is a solution to this problem it is unknown.


==List of tags with no meta information==

Unfortunatenaly some of the strings do not provide the meta information required for gender and plurality information. For instance many string that have a single number string ignore the fact someone might want to check it for plurality. So if we have {1_Num} then this just simply won't work:

<pre>{1_Num} {1:plural 1?turn; other?turns;}</pre>

With string that do not provide meta information you'll always get the first case, ie. 1 turn, 2 turn, 3 turn and not the expected 1 turn, 2 turns, 3 turns.

This is a very '''incomplete''' list of such strings.

<table class="wikitable"><tr><th>Tag</th><th>Strings</th><th>Notes</th></tr>
<tr><td>TXT_KEY_WORKER_BUILD_PROGRESS</td><td>{1_Num} {2_WorkerBuildName}</td><td>No :gender, no :plural</td></tr>
<tr><td>TXT_KEY_NEXT_POLICY_TURN_LABEL</td><td>{1_Num}</td><td>:number works, no :plural</td></tr>
<tr><td>TXT_KEY_CITY_BURNING</td><td>{1_Num}</td><td>No plural</td></tr>
<tr><td>TXT_KEY_CITY_RESISTANCE</td><td>{1_Num}</td><td>No plural</td></tr>
<tr><td>...</td><td>...</td><td>...</td></tr>
</table>
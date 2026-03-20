{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{UnknownSignature5}} Player:ChangeFaith<b>(</b><b>)</b></code>

=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
if ( iFaith > 0 ) then
    player:ChangeFaith(iFaith);
    print(player:GetName() ..": " ..iFaith .." faith from Specialists.")
end
</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeFaith]]
[[Category:Civ5 Religion API|ChangeFaith]]
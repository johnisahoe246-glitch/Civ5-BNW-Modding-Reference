''This page is a part of the [[Lua and UI Reference (Civ5)|Lua and UI Reference]].''


= About Lua =
===Lua, not LUA===
This is a Portuguese word meaning "moon", not an acronym. 


===Presentation===
Lua is an interpreted, dynamically typed, multi-paradigm language. It was designed in 1993 with the following objectives in mind:
* Extensible semantics. A small set of features allows the support of multiple paradigms, from functional programming to object programming. For example, while inheritance is not natively supported, it can be easily set up through metatables. The same features allow events in civ5 to behave both as functions and objects with Add and Remove methods.
* Highly portable. The con is a lightweight and somewhat lacking API.
* Easy to embed and to interface from other languages.
* Well suited for data description (''à la'' JSON).
* A beginners-friendly syntax.


===Performances===
As usual with interpreted and dynamically typed languages (hereby abusively named "scripting languages"), expect a 10 to 100 order of magnitude in performances decrease when compared to compiled and statically typed languages like C, C++ or C#. While it is possible for scripting languages to drastically improve the performances through more or less sophisticated means (expression trees/opcodes caching, JIT compiler, type inference to perform static resolutions), no such solution has been used in Civ5 (aside, probably, of the caching). And while an external JIT library exists, it causes compatibility problems with most mods using Lua.

That being said, Lua is still pretty good for a scripting language, better than the Python implementation from Civ4 for example. And all in all, it is fast enough for most of what modders want to achieve without the need to compromise code elegance, readability and maintainability for performances. So keep in mind that "premature optimization is the root of all evil" (Donald Knuth).


=Syntax cheatsheet=
=== Basics ===
<div class="civ5-example"><syntaxhighlight lang="lua">
-- Literals
local x = 5
local x = 5.0
local x = nil       -- A nil value is the same as an undefined value
local x = true
local x = false

-- Strings (single and double quotes can be used indifferently, there is no difference)
local x = "five"    
local x = 'five'    
local x = "five\n"  -- Escape characters with "\".
local x = [[Five is a number.
Did you know?]]     -- Multi-line string: equivalent to "Five is number.\nDid you know?"

-- Globals versus locals
x = 5               -- For globals, assigning is declaring.
local x = 5         
</syntaxhighlight></div>


=== Operators ===
<div class="civ5-example"><syntaxhighlight lang="lua">
local x = a or b
local x = a and b

local x = "hello ".."world" .. "!"    -- concatenation: two dots
local x = 4..5                        -- Result is "45". On concatenation, conversions occur.

local x = (a + b - d) * f ^ g % h     -- ^ is exponentiation, % is modulo
local x = "4" + "5"                   -- Result is 9. On arithmetic operations, conversions occur.

local x = a == b -- equality          -- True only if a and b have the same values and types.
local x = a ~= b -- inequality

local x = ((a <= b) == not (a > b)) == ((a >= b) == not (a < b))
local x = "abc" < "def"               -- Byte-wise comparison, not Unicode-compliant. Use Locale's methods instead.

local x = #"abc"                      -- Returns 3, the number of bytes in the string (3 characters, 1 byte each).
local x = #"您好世界"                   -- Returns 8, the number of bytes in the string (4 characters, 2 bytes each).
local x = #SomeTable                  -- Returns the biggest integer key in the table, or nil if there is no integer key.

-- No increment operator (++ --), no binary-assign operator (+= *=), no ternary operator (? :), no coalescence operator (??)
</syntaxhighlight></div>


=== Tables and multiple assignments ===
<div class="civ5-example"><syntaxhighlight lang="lua">
-- Table declaration
SomeTable = {}  

SomeArray = { "abc", "def" }  
    -- 1 => "abc", 2 => "def"

SomeComplexTable = { name = "John", surname = "Doe", age = 25, 43, [7] = 8 } 
    -- "name" => "John", "surname" => "Doe", "age" => 25, 1 => 43, 7 => 8.


-- Member access (all equivalent)
SomeTable.SomeMember = 5
SomeTable["SomeMember"] = 5


-- Multiple assignment
-- Both statements are equivalent since SomeArray contains "abc" and "def".
local x, y = "abc", "def"
local x, y = unpack(SomeArray) 
</syntaxhighlight></div>


=== Functions ===
<div class="civ5-example"><syntaxhighlight lang="lua">
-- Functions declarations (all equivalent)
function HelloWorld(a, b) print("Hello world") end
HelloWorld = function(a, b) print("Hello world") end    
    -- Functions are first-class objects and can be assigned like any other value!

-- Methods declarations (all equivalent)
SomeTable.HelloWorld(a, b) print("Hello world") end
SomeTable.HelloWorld = function(a, b) print("Hello world") end

-- Instanced methods declarations (all equivalent)
SomeTable.HelloWorldInstanced(self, a, b) print(self.SomeMember) end
SomeTable:HelloWorldInstanced(a, b) print(self.SomeMember) end



-- Functions and methods calls
HelloWorld(a)                  -- b will be nil in the function
HelloWorld(a, b)
SomeTable.HelloWorld(a, b)

-- Instanced methods calls (all equivalent)
SomeTable:HelloWorldInstanced(a, b)
SomeTable.HelloWorldInstanced(SomeTable, a, b)


-- Multiple return values
function func(a, b) return a, b end
local x, y, z = func(5, 6)        -- Assigns 5 to x and 6 to y, z will be nil


-- Variable arguments
function SomeFunc(a, b, ...)
   print(a)
   print(b)
   for i, v in ipairs(arg) do   -- arg is a keyword for a table containing the variable arguments
      print(v)
   end
end
SomeFunc(1, 2, 3, 4, 5)         -- prints 1, 2, 3, 4, 5
SomeFunc(1, 2)                  -- prints 1, 2
</syntaxhighlight></div>


=== Control flow ===
<div class="civ5-example"><syntaxhighlight lang="lua">
-- If 
if name == "Wu Zetian" then
    print("Hello China")
elseif name == "Napoleon" then   -- "elseif", not "else if". Beware C developers!
    print("Hello France")
else                             -- no "then" after "else"!
    print("Hello unknown")
end

-- For loop (with counter)
for i = 1, 8 do print(i) end     -- Prints 1, 2, 3, 4, 5, 6, 7, 8
for i = 1, 8, 2 do print(i) end  -- Prints 1, 3, 5, 7

-- For loop (with iterator)
for playerID, pPlayer in pairs(Players) do    -- Prints 1 Wu Zetian, 2 Napoleon, ...
    print(playerID, pPlayer:GetName()) 
end  
for plot in Plots() do                        -- Prints 0 0, 0 1, 0 2, ...
    print(plot:GetX(), plot:GetY()) 
end  

-- While (i will be 5 in the end)
while i < 5 do 
   i = i + 1
end

-- Repeat until (i will be 5 in the end)
repeat
   i = i + 1
until i == 5

-- Infinite loops
-- Lua supports "break" for all loops but not "continue" instruction does not exist!
do
   i = i + 1
   if i > 5 then break end
end

</syntaxhighlight></div>


= Basics =
=== Type system ===
You can get a variable's type by using the '''type''' function. It takes any value and returns a string. Here are all the possible results:
* The following are [http://en.wikipedia.org/wiki/Value_type value types].
** '''nil''': Lua makes do distinction between an undefined variable and a variable with a nil value. Assigning nil to a variable or table member is equivalent to undefining it.
** '''number''': a 64 bits floating-point number. Lua has no support for integers and only use floating-points. See also [[#No integer type]].
** '''boolean''': true or false obviously.
* The following are [http://en.wikipedia.org/wiki/Reference_type reference types]
** '''table''': any table.
** '''string''': your usual string of characters. In Lua all strings are interned and immutable (see [#String Interning]).
** '''userdata''': objects defined in C for use in Lua. They may not be enumerated through pairs and are often read-only. 
** '''function''': remember that functions are first-class objects in Lua.
** '''thread''': coroutines actually. Lua does not support threads.


Note: Many objects in the Civ5 API are actually regular tables which either have userdata methods as members, or a userdata metatable index.


=== Implicit conversions ===
* Whenever you concatenate two values (and possibly when you invoke a standard function that takes a string), an automatic conversion to string occurs, as if you had used the '''tostring''' function. The expression <code>4..5</code> returns "45".
* Whenever you perform an arithmetic operation, the operands are both converted to numbers, as if you had used the '''tonumber''' function. The expression <code>"4" + "5"</code> returns 9.
* The Civ5 API may or may not implicitly convert the values you pass to its methods and functions. Considers it does not.
* Aside of those, no implicit conversion is ever performed.


=== Equality comparisons ===
'''Two values are equal only if their types are the same.'''<br/>
This is far stricter than most dynamic languages for example and somehow stricter than C.
* 4 is not equal to "4". (number type and string type). In PHP they would be equal. 
* 0 is not equal to false (number type and bool type). In C they would be equal (false is typically defined as a number).
* 0 is not equal to nil. (number type and nil type). In C they would be equal (nil is typically defined as a number).


'''Numbers and booleans are compared by value. Everything else by reference. Strings are interned.'''
* Numbers and booleans are compared by value.
* Tables, userdata, functions and threads are compared by reference.
* Strings are interned (see [#String Interning]), which means that two identical strings are always the same reference. So comparisons are made by reference but are equivalent to by-value comparisons.
* All nil values are always equal.
<div class="civ5-example"><syntaxhighlight lang="lua">
local a = 5
assert(a == 5)    
-- true, comparison by value

local a = {}
assert(a == {})   
-- false, comparison by reference: those two tables are distinct objects.

local a = "Hello ".."world"
assert(a == "Hello world")
-- true, both strings are the same reference thanks to string interning.
</syntaxhighlight></div>


=== String interning ===
'''All strings are interned in Lua, without any exception.'''<br/>
[http://en.wikipedia.org/wiki/String_interning String interning] is a process through which all identical strings ends up being the same reference to a unique string instance. Typically, the interpreter maintains a string dictionary in the memory and whenever a string needs to be built (from a literal, from a concatenation, from a native call, etc), it first searches in this dictionary whether there is already a reference for this sequence of characters and uses it when it exists. This process usually reduces memory consumptions and speeds up equality comparisons, but it makes other operations slower because of the lookup cost. Some platforms such as Dotnet or Java automatically interns literals only. Lua, on the other hand, systematically interns every string.


=== Boolean logic ===
'''Anything that is neither false nor nil is evaluated to true.'''<br/>
This is pretty simple. Especially, an empty string or the zero number are evaluated to true.
<div class="civ5-example"><syntaxhighlight lang="lua">
if 0 then print("hello world") end -- prints hello world
</syntaxhighlight></div>


Now regarding the and/or operators, two rules to remember:
* '''The right operand is only evaluated when needed.'''
** <code>false and x()</code> does not call x() since the result will be false anyway.
** <code>true or x()</code> does not call x() since the result will be true anyway.
* '''The result is the last operand to have been evaluated.'''
** <code>x() and y()</code> returns x() if it was false, y() otherwise.
** <code>x() or y()</code> returns x() if it was true, y() otherwise.


=== Ternary and coalescence statements ===
We can exploit the and/or operators behavior:
* '''Coalescence:''' <code>x or y</code>. It returns x if x is neither nil nor false, y otherwise.
:In other words <code>result = x or y</code> is equivalent to: <code>if x then result = x else result = y end</code>.
* '''Ternary:''' <code>condition and x or y</code> (as long as x is not nil or false). It returns x if condition was true, y if it was false. 
:Indeed the expression becomes: <code>(condition and x) or y</code>. If condition is true the '''and''' operator returns x, and since x is true, y is not evaluated and '''or''' returns x.
:In other words <code>result = condition and x or y</code> is equivalent to: <code>if condition then result = x else result = y end</code>.


=== Method calls: dot versus colon ===
'''The colon (<code>:</code>) operator implicitly passes the caller as the first argument.''' <br/>
As opposed to the dot (<code>.</code>) operator that performs a regular call without implicitly passing anything. The colon operator behavior is obviously designed for instance methods.<br/>
<div class="civ5-example"><syntaxhighlight lang="lua">
local myTable = { msg = "Hello world" }
myTable.Print = function(self) print(self.msg)

-- Three different ways to call this method
myTable:Print() 
myTable.Print(myTable)

local func = myTable.Print
func(myTable)
</syntaxhighlight></div>


Note: in the civ5 API you will often encounter static methods that do not take any argument but that are called through a dot. This results from a misunderstanding of Lua from one of the Firaxis developers. While this work when the method does not take any argument (the one provided by the colon operator will be ignored), this is slower and can be considered as an error without any consequence.


=== Arrays versus tables ===
'''In Lua, an array is a table whose keys are integers.'''

Since this is a common programming pattern, a number of things are designed for arrays:
* <code>{"abc", "def", "ghi"}</code> starts at index 1, up to index 3. Arrays typically start at 1.
* <code>table.insert({}, "abc")</code> will transform the provided empty table to <code>{"abc"}</code>
* <code>table.insert({"abc", "def"}, "ghi")</code> will transform the provided table to <code>{"abc", "def", "ghi"}</code>
* <code>table.insert({"abc", "ghi"}, 2, "def")</code> will transform the provided table to <code>{"abc", "def", "ghi"}</code>
* <code>table.remove({"abc", "def", "ghi"}, 2)</code> will transform the provided table to <code>{"abc", ""ghi"}</code>
* <code>#{"abc", "def", "ghi"}</code> returns 3, the biggest integer key.


=== Ipairs versus pairs ===
You could say that '''pairs''' is for table and '''ipairs''' for arrays.
* '''Pairs''' enumerate all the key/value pairs in an unordered matter.
* '''Ipairs''' only enumerates the key/value pairs for consecutive integer keys, in an ascending order, starting from 1 up to the largest key. If at some point a key is missing, the enumeration stops.
::It does not matter whether the table was created with table.insert or directly by inserting the values through, for example <code>table[i] = value</code>.

<div class="civ5-example"><syntaxhighlight lang="lua">
-- Produces: { 1 => "one", 2 => "two", 4 => "four", "name" => "John", "age" => 25 }
local t = { "one", "two", name = "John", age = 25, [4] = "four" }

-- Will print (for example, the order is undetermined): "name", 2, 4, "age", 1
for k in pairs(t) do print(k) end

-- Will print 1, 2
for k in ipairs(t) do print(k) end

-- Both ipairs and pairs return a key and a value, so you could also use:
for k, v in pairs(t) do print(k, v) end
</syntaxhighlight></div>


=== Indices start at 1 ===
'''All indices in the API, not just for arrays, start at 1.'''<br/>
When you declare an array with implicit keys, when you use ipairs, when you retrieve the n-th character of a string, when you query the n-th call informations in the stack call, etcetera. This is a consistent pattern in Lua.

{{Warning}} The Civ5 API, however, uses 0-based indices, as it is the standard in C and most programming languages.


=== Semicolons and line breaks ===
'''Statements need to be separated either by a line break or a semicolon.'''
* You can use both a semicolon and a line break but then the semicolon is redundant and not required, although it does not cause any problem.
* Line breaks can also be freely added about everywhere and behave as whitespaces most of the time (you can add them after most keywords for example, so you can keep if...then...end structures on one line or split them across multiple lines).


=== Local variables visibility ===
'''Local variables are only visible after the point where they have been declared.'''<br/>
This is different from global variables that are always visible. An example is worth thousand of words.
<div class="civ5-example"><syntaxhighlight lang="lua">
function Func1()
   print(someLocal or "nil")    -- Will NOT see someLocal.
   print(someGlobal or "nil")   -- Will see someGlobal.
end

local someLocal = "foo"         -- The "foo" value will never be used.
function Func2()
   print(someLocal or "nil")    -- Will see someLocal.
   print(someGlobal or "nil")   -- Will see someGlobal.
end

someGlobal = "global"
someLocal = "local"
Func1()  -- prints "nil", then "global": someLocal is assigned but not visible from Func1
Func2()  -- prints "local", then "global": someLocal is assigned and visible from Func2
</syntaxhighlight></div>


Performances-wise, Lua first searches a variable name in the current scope, then in the parent scope, etcetera until it reaches the highest scope, and finally it searches the global scope. So the deeper a local is declared, the faster it is accessed. On the contrary, globals are the slowest to retrieve.


=== Files structure ===
* The include statement allows you to include a lua file into another one (see [[Specificities of the Lua implementation in Civ5]]). When you do so, the globals defined in the included file are imported in the parent file. However the local variables are only visible from within the file that declared them.
* If you're not familiar with scripting languages, consider that whenever Lua reads a file, it executes it. Practically, a Lua chunk (the root scope of a file) is no different from any other scope. It can contains ordinary statements as the ones found in a function scope, and you can use the <code>include</code> statement from any scope (although the globals defined in this included file will still be globals and won't be contained in the current scope). 


= Semi-advanced topics =
=== Closures ===
'''Closures are functions that embed variables that are persisted across calls.'''<br/>
This is typically achieved through a "parent" function that declares a local "closed" variable and returns another child "closure" function using this local. The "closed" variable is then unreachable for anyone but the "closure". And since it the "closed" variable is not in the "closure"'s scope, it is not reinitialized on every call of "closure".
<div class="civ5-example"><syntaxhighlight lang="lua">
function GiveMeAFunc()         -- the parent function
   local x = 0                 -- the closed variable
   return function()           -- the closure function embedding "closed"
       x = x + 1
       return closure
   end
end

local func = GiveMeAFunc()
print(func()) -- Prints 1
print(func()) -- Prints 2
print(func()) -- Prints 3
</syntaxhighlight></div>


=== Iterators ===
'''Iterators are functions for use in <code>for...in</code> loops.'''<br/>
Let's consider the following code: <code>for var1, var2, var3 in iterable() do</code>.
* iterable has the following signature: <code>iterator, state, var1 iterable()</code>. It returns a function, a state, and the initial value of var1. 
* iterator has the following signature: <code>var1, var2, var3 iterator(state, var1)</code>. It takes the state and the last value of var1 and returns var1, var2 and var3.
* The loop stops when var1 is nil.
* The for...in loop is equivalent to:
<div class="civ5-example"><syntaxhighlight lang="lua">
local iterator, state, var1, var2, var3
iterator, state, var1 = iterable()
do
   var1, var2, var3 = iterator(state, var1)
   if var1 == nil then break end

   -- Inserts here the user code defined in the for..in loop
end
</syntaxhighlight></div>
* Note that we used var1, var2 and var3 for the example but there is no restriction to the number of variables. You could have one or hundred.


Let's write the "ipairs" function.
<div class="civ5-example"><syntaxhighlight lang="lua">
local function ipairs(table)                -- The iterable function
    local iterator = function(table, key)   -- The iterator function
        key = key + 1
        return key, table[key]
    end
    return iterator, table, 0
end
</syntaxhighlight></div>


The same with closures: it's easier.
<div class="civ5-example"><syntaxhighlight lang="lua">
local function ipairs(table)                -- The iterable function
    local key = 0                           -- Both "table" and "key" are closed variables.
    local iterator = function()             -- The iterator function, a closure: it ignores the arguments provided to it
        key = key + 1                     
        return key, table[key]
    end
    return iterator                         -- No need to return anything since we do not require any argument.
end
</syntaxhighlight></div>


=== No integer type ===
'''Lua offers no support for integers and only has a 64-bits floating point number type.'''<br/>
Actually, this is only troublesome for a few algorithms that use very large integers (>2^52) or require fast integer arithmetics. But many developers misunderstand floating points and believe the problem is broader than it is. For example, does the following assertion surprise you at least a bit: "any integer smaller than 2^52 can be accurately represented with a 64-bits floating point without any error"? If it did, you suffer from some misconceptions and you should better read carefully what's coming.


Many developers are confusing rounding errors with representation errors. 
* '''Rounding errors''' actually only happen if you need a very high number of digits to represent a number. For example if you are adding a very large number with a small number. Rounding errors are very rarely encountered in day to day to applications. Actually most developers work their whole career without ever encountering them.
* '''Representation errors''' are the real problem: 0.1 is expressed in a decimal basis, but it has no finite representation in binary: it requires an infinite number of binary digits. This means that if you write 0.1 in your code it will be translated to a binary number close enough from 0.1 bot not exactly equal to it. So if you sum ten times 0.1, you sill sum ten times something close from 0.1 and the result will not be 1.


'''So the real problem for most developers only lies in the decimal-binary conversion that arises when you manipulate numbers in your code that do not have a finite representation in binary. As long as you do not use such numbers, there will be no problem. And here are the good news: integers do not suffer from any representation problem!''' Indeed, any integer can be represented with a finite number of binary digits. This is why the absence of an integer type typically does not cause problems, minus the performance penalty.


Here are a few examples to illustrate that point.
<div class="civ5-example"><syntaxhighlight lang="lua">
-- This loop works as intended: no representation error and the upper bound is far below 2^52.
local sum = 0
for i = 0, 10000000000, 1 do sum = sum + 1 end
assert(sum == 10000000001)

-- This loop works as intended: 1/16 is a floating-point with an exact representation in binary
local sum = 0
for i = 0, 1, 1/16 do sum = sum + 1 end
assert(sum == 17/16)

-- This loop does NOT work as intended: 0.1 does not have an exact representation in binary. 
-- It's the same for Lua, C and almost every programming language.
local sum = 0
for i = 0, 1, 0.1 do sum = sum + 1 end
assert(sum == 1.1) -- throws an error
</syntaxhighlight></div>


=== Errors management ===
Lua offers a error handling mechanism similar to exception handling but unfortunately not very convenient.
* Errors are thrown using the '''error''' function. It takes a string and it immediately aborts Lua execution until the game handles the error and prints it in Firetuner (when enabled).
* Errors are caught before that point using '''pcall''' or '''xpcall''', in order to let you resume execution by managing the error. "pcall" stands for "protected call".


Here are the syntaxes for pcall and xpcall:
* <code>bool, ... pcall(func, ...)</code>
** The function is called with the specified arguments.
** Pcall returns either true followed by the values returned by func, or false followed by the error text.
* <code>bool, ... xpcall(func, errorHandler)</code>:
** The function is called without any argument. If an error occurs the specified errorHandler is invoked with the error text as the only argument.
** Xpcall returns either true followed by the values returned by func, or false followed by the returned values from errorHandler.


Examples to invoke "someFunc" with "someArg" as the only argument. In both examples we want to display the error on the console, or the result if it was a success. A complete errors management example with a reporting mechanism for the end-user is presented in [[Debugging (Civ5)]].
<div class="civ5-example"><syntaxhighlight lang="lua">
-- pcall
local status, result = pcall(someFunc, someArg)
if not status then
    print("error was: "..(result or "?"))
else
    print("success: "..result)
end

-- xpcall
local status, result = xpcall(
    function() someFunc(someArg) end,
    function(err) print("error was: "..(result or "?")) end)

if status then
    print("success: "..result)
end
</syntaxhighlight></div>


= Advanced topics=
=== Metatables and metamethods ===
* Every value in Lua, from a number to a userdata, has a metatable. 
** Many objects can share the same metatable. 
** Tables and userdata each have their own metatables by default. Numbers, bools, nils and strings all share the same metatable.
* A metatable may contain a few metamethods and index tables.
** Metamethods are methods stored under special fields names. They implement operators overloads.
** Index tables behave as "base classes": if a field name is not defined on an table, then Lua looks for this field on the index.
** In a way, metatables are analogous to virtual tables in object languages, but they are not just for methods, but also for fields and operators.
* You can get an object's metatable through '''getmetatable''' and assign it with '''setmetatable'''.
* See also the [http://www.lua.org/manual/5.1/manual.html#2.8 official metatables reference]

One example.
<div class="civ5-example"><syntaxhighlight lang="lua">
-- Define two tables A and B, and set "meta" their metatable
local a, b, meta = {}, {}, {} 
setmetatable(a, meta)         
setmetatable(b, meta)

-- Define an __index table on the metatable. It contains one key/value pair.
meta.__index = { "hello world" };

-- Print "hello world" twice
print(a[1]) 
print(b[1]) 

-- Now make our tables read-only
meta.__newindex = function(table, key, value) error("this table is read-only!") end
a[1] = "foo"      -- throws an error
</syntaxhighlight></div>


Here are the most important fields a metatable can have:
* '''__index''': used when you read a member from an object. On tables, Lua will first search for a regular field on the table itself (not its index) before it looks at the index. The index may be a table or a function: <code>value func(object, key)</code>
* '''__newindex''': used when you assign a value to an object's member. On tables, newindex is only called if the table itself (not its index) does not already contains the specified key. May be a table or a function: <code>func(object, key, value)</code>
* '''__call''': used when you invoke the object as a function. Must be a function: <code>func(object, <args>)</code>
* '''__tostring''': used when you invoke the '''tostring''' function with this object in argument. Must be a function: <code>string func(object)</code>


Besides of that it can have fields for binary operators. When each of the two operands defined overloads, the left one is used. They must be functions: <code>result func(object)</code>
* '''__add''': addition
* '''__sub''': subtraction
* '''__mul''': multiplication
* '''__div''': division
* '''__mod''': module
* '''__pow''': exponentiation
* '''__eq''': equality comparison. Prior to calling this overload, Lua checks that types are equal.
* '''__neq''': inequality comparison. Prior to calling this overload, Lua checks whether types are different.
* '''__lt''': lesser than comparison. (b >= a) is considered equivalent to (a < b)
* '''__le''': lesser than or equal to comparison. (b > a) is considered equivalent to (a <= b). If __le is not defined, lua will use __lt, considering that (a <= b) is equivalent to not (b < a).
* '''__concat''': concatenation


Finally it can have the following fields for unary operators. They must be functions: <code>result func(object)</code>
* '''__unm''': unary minus
* '''__len''': the sharp operator (#). Can only be used on userdata ; on tables the default operator will always be called.


=== Implementing inheritance ===
The most common use of metatables is to mimic the behavior of object languages' types hierarchy. Here is how to do it:
<div class="civ5-example"><syntaxhighlight lang="lua">
local Dog = {}
function Dog:specie() 
   return "dog" 
end
function Dog:race() 
   return "unknown" 
end
function Dog:description()
   return self.specie().." - "..self.race() 
end
function Dog:new() 
   local instance = {}
   setmetatable(instance, { __index = self})
   return instance
end

local Pitbull = dog:new()
function Pitbull:race()
   return "pitbull" 
end

pitbull = Pitbull:new()
print(pitbull:description()) -- prints "dog - pitbull"
</syntaxhighlight></div>


This implementation is very elegant: the "new" method both creates a new instance and subtypes the creator, since "pitbull"'s index is now "Pitbull". However, should you define an operator overload on Dog's metatable, Pitbull would not inherit it. This is the limit of inheritance in Lua: operator overloads must be defined on the metatable itself, they cannot be defined on the metatable's index. As a result, there is no way to inherit those overloads while subtyping.


=== Coroutines ===
Coroutines provide a way to slice a function in many shorter calls and optionally return intermediate results. On each call, the function execution is resumed to the point where it stopped previously, with all locals being properly restored with the value they had at this time.
* Coroutines are often compared to threads. Indeed, when there are more threads than CPU cores, the operating system slices threads' execution into many little time frames and sequentially runs them in order to achieve multitasking.
* However while coroutines allows you to implement cooperative multitasking (the coroutines need to explicitly give the hand back), they cannot be used for preemptive multitasking or to use more than one system thread or CPU Core.
* As a result, coroutines are rather used as syntactic sugar (mostly to write iterators), or as a way to split a long function execution across many frames (through Context.{{Func5|UIElement|SetUpdate}}).


The following methods are mainly used:
* <code>'''coroutine''' coroutine.create('''function''' func)</code> creates a coroutine for the specified function. The function signature can be anything.
* <code>'''bool''', '''...''' coroutine.resume('''coroutine''' co, '''...''')</code> resumes the coroutine with the specified arguments. Then it returns either '''true''' followed by the returned results (either though '''return''' or '''yield'''), or '''false''' followed by an error message.
* <code>'''string''' coroutine.status('''coroutine''' co)</code> returns either "running" (the active coroutine), "normal" (a parent of the active coroutine), "suspended" (not started or waiting to be resumed) or "dead" (finished or threw an error).
* <code>coroutine.yield('''...''')</code> suspends the execution of the running coroutine and gives the hand back to the caller of coroutine.resume. The arguments will be returned by coroutine.resume.


Here is a base example:
<div class="civ5-example"><syntaxhighlight lang="lua">
function neighborsCoroutine(plot)
    for i = 0, 5 do   
        coroutine.yield(Map.PlotDirection(plot:GetX(), plot:GetY(), i))
    end
end

local co = coroutine.create(neighborsCoroutine)
while coroutine.status(co) == "suspended"
    local _, neighbor = co.resume(plot)
    -- Do something with plot
end
</syntaxhighlight></div>

Here is how to transform it into an iterator:
<div class="civ5-example"><syntaxhighlight lang="lua">
function neighbors(plot)
    local co = coroutine.create(neighbors)
    return function()
        if coroutine.status(co) ~= "suspended" then return end
        return select(2, coroutine.resume(plot))
    end
end

for neighbor in neighbors(plot) do
    -- Do something with plot
end
</syntaxhighlight></div>

Here is an example that spreads a long function call across many frames:
<div class="civ5-example"><syntaxhighlight lang="lua">
function SpreadAcrossFrames(longFunctionCall, ...)
    local co = coroutine.create(longFunctionCall)
    ContextPtr.SetUpdate(function()
        coroutine.resume(unpack(arg))
        if coroutine.status(co) ~= "suspended" then
            ContextPtr:ClearUpdate()
        end
    end)
end

SpreadAcrossFrames(SomeLongFunction, arg1, arg2)
</syntaxhighlight></div>


=== Design philosophy for Lua ===
Do not use a butter knife as you would use a chainsaw (the opposite is even more true and usually ends up badly). When designing your code, remember that:
* Lua is not an object language. While you can use objects and inheritance in some extent, you do not have to and there may be better alternatives sometimes.
* Lua is not a functional language. While you can use lambdas and similar concepts, you do not have to and there may be better alternatives sometimes.
* Lua is a multi-paradigm and dynamic language, take advantage of those.
* Lua is very suited for prototyping and small programs, and this is perfect for mods. Try to adjust your mindset: you're not writing a framework that a whole team will still use and maintain in twenty years.


[[Category:Civ5 API]]
[[Category:Civ5 Tutorials]]
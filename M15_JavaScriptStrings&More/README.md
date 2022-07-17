<h1>Module 15. JavaScript Strings</h1>
<p>|__________________________________________|</p>

<h2>I. Course Content</h2>
[]()
<>
[]()
<p>|____________________________________|</p>


<h2>_WHAT'S THE MATTER IN THIS SECTION?_</h2>
<p>|_____________________________________________________________________|</p>


<p id="goUP"></p>
<ul>
    <li><a href="#u1">1. Strings</a></li>
    <li><a href="#u2">2. Indices & Length</a></li>
    <li><a href="#u3">3. String Methods</a></li>
    <li><a href="#u4">4. </a></li>
    <li><a href="#u5">5. </a></li>
    <li><a href="#u6">6. </a></li>
    <li><a href="#u7">7. </a></li>
</ul>


<h2 id="u1">1. Strings</h2>
<p>|____________________________|</p>

```javascript
/*+-------------------------------------------------------------------------+|
* Strings;
* +-------------------------------------------------------------------------+|
* Syntax:
*   let indentifer = "value"; // double qoutes;
*   let indentifer = 'value'; // single qoutes;
+-------------------------------------------------------------------------+|
* Number as String;
*   let textNumber = "797"; // string
*+-------------------------------------------------------------------------+|
* Using another pair of quotes inside the qoutes;
* single -> double; both are valid js;
* double -> single; both are valid js;
* +-------------------------------------------------------------------------+|
* */

/*
+-------------------------------------------------------------------------+|
* Exercise;
+-------------------------------------------------------------------------+|
* bestColor should be set to purple;
* quote should have set you had me at "Hello";
+-------------------------------------------------------------------------+|
* */

let bestColor = "purple";
let quote = 'You had me at "Hello!"';
```
![introStrings](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/intoStringsJs.png?raw=true)

<h2 id="u2">2. Indices & Length</h2>
<p>|____________________________|</p>

```javascript
/*
+-------------------------------------------------------------------------+|
* Indices & Length
+-------------------------------------------------------------------------+|
* Strings are indexed(0 to n-1);
* |P| |o| |k| |e| |m| |o| |n| 
* 0    1   2   3   4   5   6
* Each character has a coresponded index number;
+-------------------------------------------------------------------------+|
* */

let animal = "Dumbo Octopus";
animal[0]; //"D"
animal[1]; //"u"
animal[4]; //"o"
animal[99]; //undefined / it's not an error
// Undefined is another Primitive DatType;

let phoneNumber = "0771402705";
phoneNumber[0]; //(


// Built-in property to figure it out what's the total amount of characters;
animal.length; // 13(not the highest index, that will be n - 1)

// Concating strings together using ' + ' operator;
"poke" + "mon" + " " + "eevee" //pokemon eevee
let firstName = "Tony";
let secondName = "Descurcaretul"
let fullName = firstName + secondName; //TonyDescurcaretul
let fullName = firstName + " " + secondName; //Tony Descurcaretul

// Concating a number and a string; will result a string;
let first = 1;
let second = "Something";
let result = firstName + second; "1Something";
typeof result; // String

```
![Indices & Length](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/IndicesLengthStringJs.png?raw=true)
![Concat with a number](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/ConcatingaNumberStringJs.png?raw=true)


<h2 id="u3">3. String Methods</h2>
<p>|____________________________|</p>

```javascript
/*
+-------------------------------------------------------------------------+|
* String Methods
+-------------------------------------------------------------------------+|
* Seaching within a string;
* Replace a part of string;
* Changing the casing of a string;
+-------------------------------------------------------------------------+|
* Syntax:
+-------------------------------------------------------------------------+|
* thing.method()
+-------------------------------------------------------------------------+|
* thing.toLowerCase(); // lowercase;
* thing.toUpperCase(); // uppercase;
* thing.Trim(); // trim whitespace from begin and end;
+-------------------------------------------------------------------------+|
* StringMethod Exercise;
+-------------------------------------------------------------------------+|
* const message = "    TASTE THE RAINBOW!  "; //DON'T CHANGE THIS LINE PLEASE!
* whisper , make the message lowercase and trim
+-------------------------------------------------------------------------+|
* */

const message = "    TASTE THE RAINBOW!  "; //DON'T CHANGE THIS LINE PLEASE!
let whisper = message.trim().toLowerCase();

```

[|_String Methods MDN Reference _|](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)

![String Methods](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/stringMethodsJs.png?raw=true)

<h2 id="u4">4. String Methods with Arguments;</h2>
<p>|____________________________|</p>


<h4> indexOf Method;</h4>

```javascript
/*
+-------------------------------------------------------------------------+|
* String Methods with Arguments;
+-------------------------------------------------------------------------+|
* this.method(argument);
+-------------------------------------------------------------------------+|
* indexOf Method;
+-------------------------------------------------------------------------+|
* this.indexOf("something");
* return the first index if found;
* return -1; if didn't found;
+-------------------------------------------------------------------------+|
*/
```

![indexof()](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/stringIndexOfMethod.png?raw=true)


<h4> replace Method;</h4>

```javascript
/*
+-------------------------------------------------------------------------+|
* replace Method;
+-------------------------------------------------------------------------+|
* thing.replace("toReplace", "tobeReplaced");
* let something = "HaHa, so funny! Tehhee";
* something.replace("Tehhee", "HaHa"); // only the first instance;
+-------------------------------------------------------------------------+|
* */
```

![replace()](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/stringreplaceMethod.png?raw=true)


<h4> slice Method;</h4>

```javascript
/*
+-------------------------------------------------------------------------+|
* slice Method;
+-------------------------------------------------------------------------+|
* this.slice(firstPos, secondPos);
* this.slice(firstPos);
* this.slice(-2); // start the slice from the last element;
* this.slice(-2,-6); // start the slice from the last element;
+-------------------------------------------------------------------------+|
* */
```
![Slice()](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/stringSliceMethod.png?raw=true)


<h4> Exercise Slice() , Replace();</h4>


```javascript
/*
+-------------------------------------------------------------------------+|
Exercise;
+-------------------------------------------------------------------------+|
* const word = "skateboard";
* use slice for board;
* use replace and change o with e;
* store it in a new varialbe;
+-------------------------------------------------------------------------+|
*/

```

![practice beard](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/stringMethodPractice.png?raw=true)

<h2 id="u5">5. String Template Literal IMPORTANT;</h2>
<p>|______________________________________________________________|</p>

```javascript
let literalString = `I Counted ${3 + 4} sheeps;`;
let result = `Your ${pokemonName} has a power of ${power}; And doubleUP to ${power * 2}`;
```

![StringTemplateLiteral](git)

<h2 id="u6">6. NULL & Undefined;</h2>
<p>|___________________________________|</p>

```javascript
/*
* NULL
*   Intentional absence of any value;
*   Must be assigned;
* 
* UNDEFINED;
*   Varibles that do not have an assigned value are undefined;
* */

// No one is loggedIn yet
let loggedInUser = null; // value explicitly nothing;
// A user logs in;
loggedInUser = 'Alan Rickman';

```
![null&Undefined](git)

<h2 id="u7">7. Math Object & Random Numbers;</h2>
<p>|___________________________________|</p>



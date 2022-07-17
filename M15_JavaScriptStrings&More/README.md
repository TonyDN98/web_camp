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
    <li><a href="#u2">2. </a></li>
    <li><a href="#u3">3. </a></li>
    <li><a href="#u4">4. </a></li>
    <li><a href="#u5">5. </a></li>
    <li><a href="#u6">6. </a></li>
    <li><a href="#u7">7. </a></li>
</ul>


<h2 id="u1">1. Strings</h2>
<p>|____________________________|</p>

```javascript
/*
* Strings;
* Syntax:
*   let indentifer = "value"; // double qoutes;
*   let indentifer = 'value'; // single qoutes;
* 
* Number as String;
*   let textNumber = "797"; // string
* 
* Using another pair of quotes inside the qoutes;
* single -> double; both are valid js;
* double -> single; both are valid js;
* */

/*
* Exercise;
* bestColor should be set to purple;
* quote should have set you had me at "Hello";
* */

let bestColor = "purple";
let quote = 'You had me at "Hello!"';
```
![introStrings](https://github.com/TonyDN98/web_camp/blob/main/M15_JavaScriptStrings&More/ss/intoStringsJs.png?raw=true)

<h2 id="u2">2. Indices & Length</h2>
<p>|____________________________|</p>

```javascript
/*
* Indices & Length
* Strings are indexed(0 to n-1);
* |P| |o| |k| |e| |m| |o| |n| 
* 0    1   2   3   4   5   6
* Each character has a coresponded index number;
* */

let animal = "Dumbo Octopus";
animal[0]; //"D"
animal[1]; //"u"
animal[4]; //"o"
animal[99]; //undefined / it's not an error
// Undefined is another Primitive DatType;

let phoneNumber = "0771402705";
phoneNumber[0]; //(


// Build-in property to figure it out what's the total amount of characters;
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



<h2 id="u3">3. String Methods</h2>
<p>|____________________________|</p>




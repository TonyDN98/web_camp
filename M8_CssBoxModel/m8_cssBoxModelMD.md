<style>
h1,h2,h3,p,a {
    font-family: Verdana,monospace;
    color: pink;
    
}
</style>

<h1>Module 8. Css BoxModel</h1>
<p>|__________________________________________|</p>

<h2>I. Course Content</h2>


[m8_cssBoxModel.html HTML File](m8_cssBoxModel.html)<br>
[m8_cssBoxModelStyle.css CSS File](m8_cssBoxModelStyle.css)

<p>|____________________________________|</p>


<h2>II. Practice Content</h2>

<p>|____________________________________|</p>



<p>|____________________________________|</p>



<h2>_WHAT'S THE MATTER IN THIS SECTION?_</h2>
<p>|_____________________________________________________________________|</p>

<p id="goUP"></p>
<ul>
    <li><a href="">1. BoxModel Width & Height</a></li>
    <li><a href="">2. Border \ Border-Radius</a></li>
    <li><a href="">3. Padding</a></li>
    <li><a href="">4. Margin </a></li>
    <li><a href="">5. Display Property IMPORTANT </a></li>
    <li><a href="">6. CSS UNITS IMPORTANT</a></li>
    <li><a href="">7. CSS UNITS: ems </a></li>
    <li><a href="">8. CSS UNITS: rems </a></li>
</ul>



<h2>1. Width & Height</h2>
<p>|____________________________|</p>

```css

/*
+-------------------------------------------------------------------------+|
| WIDTH & HEIGHT
| Width (LEFT / RIGHT)
| Height (UP / DOWN)
|+-------------------------------------------------------------------------+
```

```html
<div class = "divclass"></div>
<div class = "divclass"></div>

```

```css
.divclass {
    width: 200px;
    height: 200px;
}
```

<h2>2. Border / Border-Radius</h2>
<p>|____________________________|</p>

```css
/*
BORDER
border-width >- control thickness of the border
border-color >- color of border
border-style >- style - dashed, solid, etc;

ShortHand
border:border-width border-color border-style

border-radius(rounded corners): use relative values, px it's not a good idea for this situation;
 */
```

```html
<div id="three">
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
        Accusantium eum eveniet, illo iure laudantium magnam nesciunt non quia voluptas?
        A consequuntur debitis distinctio eum ipsum laboriosam mollitia odit velit voluptatem.
    </p>
</div>
```

```css
#three {
    background: #6d6875;
    /*width | style | color*/
    border: 2px dashed red ;
    border-radius: 15%;
}
```

<h2>3. Padding</h2>
<p>|____________________________|</p>

```css
/*
PADDING
Padding is the space between the content and thr border;

border
|---------------------------------------|border
|              PADDING                  |
|        -------------------            |
|PADDING|     CONTENT      |  PADDING   |
|       |     BOX          |            |
|       ---------------------           |
|             PADDING|                  |
|---------------------------------------|
border

padding-left
padding-right
padding-bottom
padding-top

Shorthand Padding:
padding: 10px; All 4 sides

Vertical | Horizontal
padding 5px 10px;

Top | Right | Bottom | Left | around the clock
padding: 1px 2px 3px 4px;
 */
```


```html
<div>
    <button>Click me</button>
</div>
```

```css
div button {
    /*padding: 20px;*/
    /*padding: 10px 20px;*/
    padding: 10px 20px 30px 40px;
}
```

<h2>3. Margin</h2>
<p>|____________________________|</p>

```css
/*
Margin
Margin is the space between other elements;
                ELEMENT 1                                                   ELEMENT 2
|-------------------------------------------------------| |-------------------------------------------------------|
|                   MARGIN                              | |                   MARGIN                              |
|      |----------border------------------------| MARGIN| |      |----------border------------------------| MARGIN|
|MARGIN|              PADDING                   |       | |MARGIN|              PADDING                   |       |
|      |        -------------------             |       | |      |        -------------------             |       |
|      |PADDING|     CONTENT      |  PADDING    |       | |      |PADDING|     CONTENT      |  PADDING    |       |
|      |       |     BOX          |             |       | |      |       |     BOX          |             |       |
|      |       ---------------------            |       | |      |       ---------------------            |       |
|      |             PADDING|                   |       | |      |             PADDING|                   |       |
|      |---------------border-------------------|       | |      |---------------border-------------------|       |
|                   MARGIN                              | |                   MARGIN                              |
|-------------------------------------------------------| |-------------------------------------------------------|

margin-left;
margin-right;
margin-bottom;
margin-top'

Shorthand Margin:
margin: 10px; All 4 sides

Vertical | Horizontal
margin: 5px 10px;

Top | Right | Bottom | Left | around the clock
margin: 1px 2px 3px 4px;
*/
```


```css
/*It's a good idea to take your margin off for body, to get that extra space;*/
body{
margin:0px;
}
```

<h2>4. display</h2>
<p>|____________________________|</p>

```css
/*
display:none >- hide an element;
display:inline >- change properties of an block-level element to be  displayed inline
display: block >- change properties of an inline element to be  displayed block-level
display: inline-block >- generate a block element that will be flowed with surrounding content as if it where a singe inline block 

*/
```

```html
<div class="divdisplay"></div>
<div class="divdisplay"></div>
<div class="divdisplay"></div>

<div class="displaynone">
    <p>This will disappear;</p>
</div>
```

```css
.divdisplay{
    height: 200px;
    width: 200px;
    background-color: olive;
    border: 5px solid black;
    display: inline-block;
    margin: 10px;
    padding: 10px;
}

.displaynone{
    display: none;
}
```


<h2>5. display</h2>
<p>|____________________________|</p>

```css
/*
% unit;
 they  are going to be % of the parent element;


Em Units use relative from the parent element
Rem Units use relative from root element;

Working with fonts;
font unit, will be 2x font size of the parent element;

padding, margin;
1em or 2em will be 2x the size of the element it self;
```









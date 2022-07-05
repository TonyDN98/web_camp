<h2 id="u1">x. FLEX-SIZING Properties;</h2>
<p>|_________________________________________|</p>

<h3>flex-basis</h3>
<p>|________________|</p>

```css
/*
|----------------------------------------------------------------------------------|
| 1. FLEX-BASIS
| * Define initial size of an element before additional space distribution;
|----------------------------------------------------------------------------------|
*/

#container div:nth-of-type(2){
    flex-basis: 400px;
}
```

<h3>flex-grow</h3>
<p>|________________|</p>

```css
/*
|----------------------------------------------------------------------------------|
| 2. FLEX-GROW
| * Control the amount of available space an element should take up; 
| * We telling how much to grow according to the other elements;  
| * Accepts a unit-less number value: 1, 2, 3
|----------------------------------------------------------------------------------|
*/

#container div:nth-of-type(2){
    flex-basis: 400px;
    flex-grow: 1;
}
```


<h3>flex-shrink</h3>
<p>|________________|</p>

```css
/*
|----------------------------------------------------------------------------------|
| 3. FLEX-SHRINK
| * If items are larger then the container , they shrink according to flex-shrink;
| * We telling how much to shrink according to the other elements;  
| * Accepts a unit-less number value: 1, 2, 3
|----------------------------------------------------------------------------------|
*/

#container div:nth-of-type(3){
    flex-basis: 400px;
    flex-grow: 1;
    flex-shrink: 2;
}
```


```html
<main>
    <div class="sidebar"></div>
    <div class="maincontent"></div>
</main>
```

<h3>Flex Shorthand</h3>
<p>|____________________|</p>

```css
/*
|----------------------------------------------------------------------------------|
| 4. FLEX SHORTHAND;
|flex : flex-grow | flex-shrink | flex-basis;
|----------------------------------------------------------------------------------|
*/

main{
    width: 80%;
    margin: 0 auto;
    border: 5px solid black;
    height: 500px;
    /*Starting flex*/
    display: flex;
}

main .sidebar{
    background-color: #6930c3;
    flex: 1 2 300px;
}

main .maincontent{
    background-color: #80ffdb;
    flex: 2 600px;
}
```


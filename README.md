

### Front End Development
#### Front End Development Languages
  - ##### HTML (Hyper Text Markup Language)
  - ##### CSS (Casecading Style Sheet)
  - ##### Java Script 

## HTML (Hyper Text Markup Language)
## CSS (Casecading Style Sheet)

### CSS Units

| Unit Name |  Relative to | Standard/Default Values | 
| ---- | --- | --- |
| px   | dpi | 1px = 2.54 dpi | 
| em   | Parent Element | 1em = 16px  |
| rem   | Root Element | 1rem = 16px |
| %  | Parent Element | 100% = 16px |
|vw   | Viewport's Width | 1vw = 4.8px or 1% of viewport width |
| vh   | Viewport's Height | 1vw = 8px or 1% of viewport height |

#### 

### CSS Variables
 - Help in organizing the style 
 - Can be reused
 - ```var()``` function is used to insert the value of a CSS variable, it's syntax look like this:
 ``` 
  var(--name, value)
 ```
Note: Variable name is required and must start with two dashes, variable value is optional, this is fallback value and used when variable not found.
 - CSS variables have the access to DOM
 - ```:root``` Selector is used to declare the variables in CSS (`:root` Selector is the highest level of selector in CSS)
 Syntax for declaring variable looks like this:
 ```css
 :root {
  --maincolor: #ffffff;
  --sectioncolor: #000000;
 }
section {
 background-color: var(--sectioncolor);
}

 ```
   > Resources: [freeCodeCamp](https://www.freecodecamp.org) RWD Curriculum, [W3School](https://www.w3schools.com)


### CSS Comments
  We can comment in CSS as below:
```css
 /* Comment Here */ 
```
### Media Query

A media query can be used to change styles based on certain conditions, and they look like this:
```css
@media (condition) {

}  
````
### CSS Gradient
- Gradients in CSS are a way to transition between colors across the distance of an element
- CSS defines different types of gradients:
  - Linear Gradients (goes down/up/left/right/diagonally)
  - Repeating Linear Gradients (gradient repeat until it gets to the bottom of the element)
  - Radial Gradients (defined by their center)
  - Conic Gradients (rotated around a center point)
- They are applied to the background property
- Syntax for Gradients look like this:
```css
  gradient-type(
    direction,
    color1,
    color2
    );
```  
 In the example, color1 is solid at the top, color2 is solid at the bottom, and in between it transitions evenly from one to the next. Default dircetion of the linear gradient is from top to bottom. We can specify the direction by putting the value like ```90deg```.  ``` circle closest-corner at 15% 15%, ``` is an example for using direction for ```radial-gradient```. This will move the start of the gradient to 15% from the top and left. It will make it end at the closest-corner and it will maintain a circle shape.

 You can specify where you want a gradient transition to complete by adding it to the color like this:
```css 
gradient-type(
  color1,
  color2 20%,
  color3
);
```
Here, it will transition from color1 to color2 between 0% and 20% of the element and then transition to color3 for the rest.

Gradient transitions often gradually change from one color to another. You can make the change a solid line like this:
```
linear-gradient(
  var(--first-color) 0%,
  var(--first-color) 40%,
  var(--second-color) 40%,
  var(--second-color) 80%
);

``` 
   > Resource [freeCodeCamp](https://www.freecodecamp.org)
 RWD Curriculum, [W3School](https://www.w3schools.com)


## Java Script


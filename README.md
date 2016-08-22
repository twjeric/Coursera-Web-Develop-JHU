# Web Front End Design Resources

https://sarasoueidan.com/index.html

About SVG: https://www.w3.org/TR/SVG/coords.html#EstablishingANewUserSpace

# Coursera-Web-Develop-JHU

browser-sync start --server --directory --files "*"

HTML Character Entity References:
1.<    &lt;
2.>    &gt;
3.&    &amp;
4.non breaking space &nbsp;
5.quote &quot;
6.copyright &copy;

a标签中 target="_blank" 则链接在新标签页中打开

Combining Selectors:
- Element with class selector (selector.class)
- Child (direct) selector (selector > selector)
- Descendent selector (selector selector)
- Adjacent sibling selector (selector + selector)
- General sibling selector (selector ~ selector)

Pesudo-Class Selectors:
- :link
- :visited
- :hover
- :active
- :nth-child(3) nth-child(odd)

Specificity：!important > style="..." > ID > Class,pesudo-class,attribute > # of elements

Style:
```css
<style>
body {
font-family: Arial, Helvetica, sans-serif;
color: #0000ff;
font-style: italic;
font-weight: bold;
font-size: 24px; default:16px;
text-transform: uppercase;
text-align: right;
}
</style>
style="font-size: 2em;" m大小的两倍
```

The Box Model
![](https://github.com/twjeric/Coursera-Web-Develop-JHU/blob/master/The%20Box%20%20Model.png)
width is set to the content by default, not the box size;

change it by using box-sizing: border-box (non-inherited)
```css3
* {
   box-sizing: border-box;
}
```
verticle margin will collapse, the larger margin of two elements wins
overflow: auto;

![Media Query Syntax](https://github.com/twjeric/Coursera-Web-Develop-JHU/blob/master/Media%20Query%20Syntax.png)
![Responsive Web Site](https://github.com/twjeric/Coursera-Web-Develop-JHU/blob/master/Responsive%20Web%20Site.png)

Viewport meta tag to turn off default mobile zooming
```css3
<meta name="viewport" content="width=device-width, initial-scale=1">
```

Bootstrap Grid System Basics
```html
<header class="container">
  <nav class="row">
    <div class="col-md-4">Col 1</div>
    ...
  </nav>
</header>
```

Website Links:
- http://getbootstrap.com/
- https://jquery.com/
- http://placehold.it/
- https://scotch.io/tutorials/open-sublime-text-from-the-command-line-using-subl-exe-windows
- http://olivierlacan.com/posts/launch-sublime-text-3-from-the-command-line/
- http://ajaxload.info/

Javascript
```javascript
if ( false || null || undefined || "" || 0 || NaN) {
  console.log("This line won't ever execute");
}
else {
  console.log("All false");
}

if (true && "hello" && 1 && -1 && "false") {
  console.log("All true");
}

//Regular(==) and Strict(===) Equality

//Handling default values
sideDish = sideDish || "whatever!";

//object literal
var facebook = {
  name: "Facebook",
  ceo: {
    firstName: "Mark",
    favColor: "blue"
  },
  "stock of company": 110
};

//Function constructors
function Circle (radius) {
  this.radius = radius;
}
Circle.prototype.getArea = function () {
  return Math.PI * Math.pow(this.radius, 2);
};
var myCircle = new Circle(10);
console.log(myCircle.getArea(10));

//Object literals and "this"
var literalCircle = {
  radius: 10,
  
  getArea: function () {
    var self = this;
    
    var increaseRadius = function () {
      self.radius = 20;
    };
    increaseRadius();
    
    return Math.PI * Math.pow(this.radius, 2);
  }
};

console.log(literalCircle.getArea());

//Arrays
var array = new Array();
var names = ["tang","wei","jie"];
for (var i = 0; i < names.length; i++) {
  console.log("Hello " + names[i]);
}
var myObj = {
  name: "Yaakov",
  course: "HTML/CSS/JS",
  platform: "Coursera"
};
for (var prop in myObj) {
  console.log(prop + ": " + myObj[prop]);
}
for (var name in names) {
  console.log("Hello " + names[name]);
}

//
function makeMultiplier (multiplier) {
  return (
    function (x) {
      return multiplier * x;
    }
  );
}
var doubleAll = makeMultiplier(2);
console.log(doubleAll(10));

//Immediately Invoked Function Expression
//IFEE
(function (name) {
  console.log("Hello " + name);
})("Coursera!");
```

Ajax
![](https://github.com/twjeric/Coursera-Web-Develop-JHU/blob/master/How%20Does%20Ajax%20Work.png)
![](https://github.com/twjeric/Coursera-Web-Develop-JHU/blob/master/Ajax%20Process.png)

# Github-Flavored-Markdown

A task list
- [X] Write the code
- [ ] Write all the tests
- [ ] Document the code

Code Snippets
```java
for(int i=0 ; i < 5 ; i++)
{
   System.out.println("i is : " + i);
}
```

Quoting
> Whether 'tis Nobler in the mind to suffer

> The Slings and Arrows of outrageous Fortune,

How big are these slings and in particular, these arrows?

Emoji

I :eyes: that :bug: and I :cold_sweat:.

:trophy: for :microscope: it.

:+1: and :sparkles: on this :ship:, it's :fire::poop:!

:clap::tada::panda_face:

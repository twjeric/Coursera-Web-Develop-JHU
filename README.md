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

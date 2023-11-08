HTML : Content and structure of website
CSS : Styling and positioning of contents
JS : Interactivity and behavior of website structures

# HTML

> References : https://developer.mozilla.org/en-US/docs/Web/HTML/Element

The homepage should always be mentioned as `index.html`. This is because every server always look for the `index` name when a client requests a webpage

#### Head

It contains meta information. Must not contain any content

#### Attributes

They are placed within element tags such as `<a href="a_value">Click on this link</a>`

An attribute consists of a name and a value, and is placed inside tags to extend functionality of an element.

# CSS

Div : group elements together as blocks. The elements are enclosed in a container. (block-level element)

span : group text or inline-elements 

### List of block elements
```html
<address>
<article>
<aside>
<blockquote>
<canvas>
<dd>
<div>
<dl>
<dt>
<fieldset>
<figcaption>
<figure>
<footer>
<form>
<h1>-<h6>
<header>
<hr>
<li>
<main>
<nav>
<noscript>
<ol>
<p>
<pre>
<section>
<table>
<tfoot>
<ul>
<video>
```


### List of inline elements
``` html
<a>
<abbr>
<acronym>
<b>
<bdo>
<big>
<br>
<button>
<cite>
<code>
<dfn>
<em>
<i>
<img>
<input>
<kbd>
<label>
<map>
<object>
<output>
<q>
<samp>
<script>
<select>
<small>
<span>
<strong>
<sub>
<sup>
<textarea>
<time>
<tt>
<var>
```

## Box
Every elements are enclosed in a box. That is why in old websites, elements appeared as stacked on top of one another.

## Inline
In inline, the elements can be set on the same line but the height and width are ignored and only the top and bottom padding are considered. See example below. 
![a4e253d3479d40a8883f79adb398706c.png](../_resources/a4e253d3479d40a8883f79adb398706c.png)

## block
In block, each element begins one new line. i.e. Appears as blocks stacked on top of one another
![c27112f0f73da2434ef7b88d98c86ad1.png](../_resources/c27112f0f73da2434ef7b88d98c86ad1.png)

### Inline-box
Inline box is a mixture of inline and block where all are considered, including the heigh, width and paddings. 
![89a332b22636a55a46b02b48bf06e35f.png](../_resources/89a332b22636a55a46b02b48bf06e35f.png)

### Flex
A flex container and a flex item are 2 parts of Flex.

An element can be made a flex container, holding other elements known as flex items. 

```HTML
<div class="flex-container">
  <div class="one"></div>
  <div class="two"></div>
  <div class="three"></div>
</div>
```

Here, we can see the nested divs as a flex structure. The `first div` will be made a `flex container` holding the `nested divs` as `flex items`.

```CSS
.flex-container {
  display: flex;
}

/* this selector selects all divs inside of .flex-container */
.flex-container div {
  background: peachpuff;
  border: 4px solid brown;
  height: 70px;
  flex: 1;
}
```

A flex container is declared by writing `display: flex` 

> A flex item can also be made a flex container. This dual nature is what allows flex to build complex layouts. 

Flex is a shorthand for 3 properties, where `flex: 1` is equal to `flex grow: 1` , `flex shrink: 1`, `flex basis: 0`.   
1. Flex grow:  It only applies when proportion t of flex items flex container
2. Flex shrink: This allows shrinking of flex items in proportion to the flex container. It only applies when total size of flex items are greater than the flex container they are inside of
3. Flex basis: the baseline from which flex items starts to grow or shrink.  If set to `auto`, the baseline is the width/height values declared.  
## JS 

# Backend

> Preferable languages are Python, Ruby and PHP
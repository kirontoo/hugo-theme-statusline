---
title: "Markdown Guide"
date: 2020-06-09T16:06:02-07:00
author: amy dang
draft: true
categories: [ "guide" ]
tags: [ "markdown" ]
series: []
description: "A sample article to showcase basic Markdown syntax and formatting for HTML elements."
---

This a sample article that will show how Markdown syntax can be used in Hugo content files
and how basic HTML elements are styled with CSS in this Hugo theme.

# Headings
This is how headings are rendered. There are six levels of section headings. `<h1>` is the highest while ``<h6>`` is the lowest.

# H1
## H2
### H3
#### H4
##### H5
###### H6

# Paragraphs
Lorem ipsum dolor sit amet, consectetur adipiscing elit. In dapibus orci et luctus gravida. Nunc luctus condimentum elit nec euismod. Duis eget eros ac massa eleifend feugiat. Morbi finibus odio porttitor nulla mollis, in posuere purus ultrices.

Nunc vitae laoreet lectus. Curabitur viverra venenatis porta. Fusce luctus eros eu purus tristique facilisis. Duis in libero non turpis sodales viverra. Vivamus tempus, metus sit amet consectetur tempor, enim risus venenatis mi, a ornare lorem massa vel dui. Fusce luctus semper euismod. Nullam non efficitur nisl. 

# Emphasis
italic: *this text will be italic*

bold: **this text will be bold**

# Inline code
Inline code blocks can be used like `this`.

# Blockquotes
Blockquotes can be made with or without citations. Citations can be found at the bottom of the page.

## Blockquote without citation
> Lorem ipsum dolor sit amet, consectetur adipiscing elit.
> 
> **Note** you can also use markdown syntax inside a blockquote

## Blockquote with citation

>“Lesser, greater, middling, it's all the same. Proportions are negotiated, boundaries blurred. I'm not a pious hermit, I haven't done only good in my life. But if I'm to choose between one evil and another, then I prefer not to choose at all.”</p>
>
> — <cite>Andrzej Sapkowski, The Last Wish[^1]</cite>
[^1]: The above quote is excerpted from Adrezei Sapkowski's book "The Last Wish"

# Lists
## Unorderd
* Item 1
* Item 2
* Item 3

### Nested
* Item 1
	* Nested item
* Un-nested item

## Ordered list
1. Item 1
2. Item 2
3. Item 3

### Nested list
1. Item
	1. Nested item
2. Un-nested item

# Images
Image can be linked by a URL or by the image's source path. Images can also be captioned.

## Image without caption
![hammer head keycaps](/images/hammerhead.jpg)
## Image with caption
![hammer head keycaps](/images/hammerhead.jpg "This is a image caption")

# Links
this is how a [link](https://www.gohugo.io "Title") works.
Any URL like this http://www.github.com/ will automatically be turned into a link.

# Tables
Markdown does not natively support tables but Hugo does.

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

## Tables with Inline Markdown 
First Header | Second Header
------------ | -------------
*italic*     | **bold text**
~~strikethrough~~ | ``code``

# Task Lists
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

# Code Blocks and Syntax Highlighting

## Code block with backticks
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

## Code block Using indentation
		function fancyAlert(arg) {
			if(arg) {
				$.facebox({div:'#foo'})
			}
		}

## Code block with Hugo's built-in highlight shortcode
{{< highlight javascript >}}
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
{{< /highlight >}}


# Miscellaneous 
Subscripts, superscripts, abbreviations, keyboard commands, marks ( highlight ) can be used only if `markup.goldmark.renderer.unsafe` is enabled.
You can change the text color by adding `class="your-color" `to the HTML tags. 

**Example**: 
`H<sub class="yellow">2</sub>0` will output H<sub class="yellow">2</sub>O

Colors available:
* <span class="red">red</span>
* <span class="orange">orange</span>
* <span class="yellow">yellow</span>
* <span class="green">green</span>
* <span class="blue">blue</span>
* <span class="purple">purple</span>
* <span class="pink">pink</span>
* <span class="cyan">cyan</span>

## Abbreviations
<abbr class="green" title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

## Subscript 
H<sub>2</sub>O

## Superscript
X<sup>n</sup> + Y<sup>n</sup>: Z<sup>n</sup>

## Keyboard commands
Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

## Marks
Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

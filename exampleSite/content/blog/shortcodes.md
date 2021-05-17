---
title: "Shortcodes"
date: 2020-06-17T10:58:31-07:00
author: kirontoo
categories: [ "guide" ]
tags: [ "shortcodes" ]
series: [ "hugo-guide" ]
draft: false
description: "Here are a few custom shortcodes I created for your use!"
summary:
---

Here are a few custom shortcodes I created for your use!


# Headings
`NOTE:` these headings will not show up on the table of contents

{{< h1 "h1 heading" >}}
{{< h2 "h2 heading" >}}
{{< h3 "h3 heading" >}}
{{< h4 "h4 heading" >}}
{{< h5 "h5 heading" >}}
{{< h6 "h6 heading" >}}

{{< h1 "h1 heading stretched" stretch>}}
{{< h2 "h2 heading stretched" stretch>}}
{{< h3 "h3 heading stretched" stretch>}}
{{< h4 "h4 heading stretched" stretch>}}
{{< h5 "h5 heading stretched" stretch>}}
{{< h6 "h6 heading stretched" stretch>}}

# Images With Custom border style
Will work with local files and image src links.
### Image with no border style
{{< image src="https://i.redd.it/tgpnsvzmui651.jpg" alt="text" caption="title" color="cyan">}}
### Image with bracket style
{{< image src="https://i.redd.it/tgpnsvzmui651.jpg" caption="my caption" style="bracket">}}
### Image with border style
{{< image src="images/hammerhead.jpg" caption="my caption" style="border" color="orange" >}}


# Colors
Colors available:
* {{< colored "red" red >}}
* {{< colored "orange" orange >}}
* {{< colored "yellow" yellow >}}
* {{< colored "green" green >}}
* {{< colored "blue" blue >}}
* {{< colored "purple" purple >}}
* {{< colored "pink" pink >}}
* {{< colored "cyan" cyan >}}
* {{< colored "white" white >}}

## Color your text!
Use the  `colored` shortcode to color your text!

Demo: {{< colored "yellow colored text" yellow >}}

Syntax: `<colored "my text here" your_color>`

## Colored Inline-code

Default inline-code: {{< inline-code "my text" >}} with inline-code.

Custom inline-code: {{< inline-code "my purple text" purple >}} with inline-code.

Syntax: `< inline-code "your text here" your_color >`

## Change blockquote border color
Use `blockquote` to customize the border and text color.
{{< blockquote  border="yellow" color="cyan" text="custom blockquote" >}}

Syntax: ```< blockquote border="your_color" color="your_color" text="your text here" >```

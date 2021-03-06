---
title: Working w/ Markdown (Fix me!)
date: '2019-01-09'
tags: ['Dev', 'Content', 'MD', 'Markdown']
slug: working-with-markdown
image: ./images/bg-image-5.jpg
image_caption: ---
flip: false
dirction: ltr
excerpt: Hearing a lot of Markdown but don't know where to begin? Here's a good spot
---

# Basics

Notion is made out of `blocks` of content

This line, *now marked in purple*, is a block 

But **you can** use **`inline` styling as ~~well~~**, i.e. style inside a `text element`. 

Create blocks by pressing the `/` key, or use the *plus icon* on the left of each block, while hovering  

<!-- <div class="full-width-cont"> -->

<div class="--split-2">

<div>

![Blinking picxel Kof](https://media.giphy.com/media/klAeYVG0SOYYUqDS9h/giphy.gif){class="post--img"}

The hover *plus icon*

</div>

<div>

You can easily create grids like the one you're now viewing by dragging and dropping `blocks` of content

Grids stack differently in web then mobile. This is how:

</div>

</div>

<!-- </div> -->

![Working%20w%20Notion/Grids_in_notion.jpg](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/aaffe686-c634-4715-9673-fb56c80b9d76/Grids_in_notion.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20200520%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20200520T130724Z&X-Amz-Expires=86400&X-Amz-Signature=28e38a6a89e6aec105c4cf245773cb0bb286efb19ec191d2ea821a4f32828a81&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Grids_in_notion.jpg%22)

> **Keep in mind →** Everything in Notion is changeable, movable and editable, reversible and indestructible. So don't be afraid to explore!

### **`* In a way`**
---

Be sure to read more over at the Notion's documentation, here's the link 👇 

[Help & Support](https://www.notion.so/Help-Support-e040febf70a94950b8620e6f00005004)


Types of grouping

**This is a group - using tabs**

I'm a child 

Another child

1. **This is a group - using bullets**
1. I'm a child
1. Another  

- **This is a group - using bullets**
- I'm a child
- Another child **This is a group - using multiple** 
- I'm a child

1. Another  
1. Another  
1. Another  

---

[Try 1](https://www.notion.so/b1d2f64f478f44aa859cfb78134c3784)

[Sum of Try 1](https://www.notion.so/2221d484d74a439ea74b129c29a21ff1)

[Try 2](https://www.notion.so/97b6bf2d25ae4b9c8211fd73a0b5b7cb)

# Notion Formulas

if(prop("Days overdue") > 365, "More then an year", if(prop("Days overdue") > 90, "More then a quter", if(prop("Days overdue") > 30, "More then a month", if(prop("Days overdue") > 7, "More then a week", if(prop("Days overdue") > 0, "This week", "Missed this one")))))

[Notion Formulas](https://www.notion.so/Notion-Formulas-ec27b88ceb864aaeb08c6ab003b350ca)

[Notion Formulas: The ultimate reference guide (with templates)](https://radreads.co/notion-formulas/)

---

Colons can be used to align columns.

| Tables          | Are             | Cool  | and      | are       | Pretty      |
| --------------- | --------------- | ----- |---       | ---       | ---         |
| col 3 is        | right-aligned   | $1600 | *Still*  | `renders` | nice  |
| col 2 is        | centered        |   $12 | 1        | 2         | 3           |
| zebra stripes   | are neat        |    $1 | 100      | 2000      | 9349        |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

| Markdown | Less      | Pretty      |
| ---      | ---       | ---         |
| *Still*  | `renders` | **nicely**  |
| 1        | 2         | 3           |
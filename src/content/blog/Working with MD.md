---
title: Working w/ Markdown (Fix me!)
date: '2019-01-09'
tags: ['Dev', 'Content', 'MD', 'Markdown']
slug: working-with-markdown
image: ./images/bg-image-5.jpg
flip: false
dirction: ltr
excerpt: Hearing a lot of Markdown but don't know where to begin? Here's a good spot
---

# Basics

Notion is made out of `blocks` of content

This line, *now marked in purple*, is a block 

But **you can** use **`inline` styling as ~~well~~**, i.e. style inside a `text element`. 

Create blocks by pressing the `/` key, or use the *plus icon* on the left of each block, while hovering  

![Working%20w%20Notion/Screen_Shot_2019-08-15_at_13.27.51.png](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/ac4110f8-149f-4cdb-9efe-6742be60fc7f/Screen_Shot_2019-08-15_at_13.27.51.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20200423%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20200423T135035Z&X-Amz-Expires=86400&X-Amz-Signature=f7c2513af9fc9337ac7b02b1a270b62c4737220d4929fe536b55146d90653db1&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Screen_Shot_2019-08-15_at_13.27.51.png%22)

The hover *plus icon*

You can easily create grids like the one you're now viewing by dragging and dropping `blocks` of content

Grids stack differently in web then mobile. This is how:

![Working%20w%20Notion/Grids_in_notion.jpg](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/aaffe686-c634-4715-9673-fb56c80b9d76/Grids_in_notion.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20200423%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20200423T134929Z&X-Amz-Expires=86400&X-Amz-Signature=6fb270b8d1b40c46ae902fd0714619515fdca03c943b564a4cada0d9c4924ac8&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Grids_in_notion.jpg%22)

> **Keep in mind →** Everything in Notion is changeable, movable and editable, reversible and indestructible. So don't be afraid to explore!

### **`* In a way`**
---

Be sure to read more over at the Notion's documentation, here's the link 👇 

[Help & Support](https://www.notion.so/Help-Support-e040febf70a94950b8620e6f00005004)

![Blinking picxel Kof](https://media.giphy.com/media/klAeYVG0SOYYUqDS9h/giphy.gif)

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
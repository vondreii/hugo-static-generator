---
title: "Content"
date: 2020-11-17T15:05:56+05:30
draft: false

categories: ["Hugo"]
icon: "fas fa-fire-alt"
---

## Content

Each post is going to be written in a separate markdown file.
For example, if you wanted to write something on Chocolate Lava Cakes, you would have a file called `ChocolateLavaCake.md` where you would write your text.

The hugo-sugoi theme comes with some examples. Navigate to `my-food-blog\themes\hugo-sugoi\exampleSite`. There you will see a folder called `content`.

Copy this `content` folder and paste it into the `my-food-blog` folder, where the root of the project is (overwrite the existing one). 

Run the program again:

```
hugo serve

```

Now you have some content!

Go into `my-food-blog\content\post` and observe the 4 markdown files that represent the 4 posts:
-  air-nation-list-style.md
-  code-blocks.md
-  prince-zuko.md
-  water-nation-pride-and-peace.md

You can open any one of them to see the format of how you need to write your posts in Markdown.

In a Markdown file, you can just write the content as plain English - like you would on Microsoft Word - except you can use symbols to signify headings or special styling in your text. For example:

`# Something` is a main heading, like this:  

# Something 

<br>

`## Something` is a next level sub heading, like this:  

## Something 

<br>

`### Something` is an even lower sub level heading, like this: 

### Something

<br>

`**Something**` Will make something bold, like this: **Something** 

`*Something*` Will make something italicized, like this: *Something* 

`[Something](https://www.google.com)` is a link: [Something](https://www.google.com)

There are a few places where you can read some of the syntax used for markdown:
* https://www.markdownguide.org/basic-syntax/
* https://www.markdownguide.org/cheat-sheet/

Now everytime you want to start a new post, all you have to do is write it in a new `Markdown` file, inside the `content/post` folder!
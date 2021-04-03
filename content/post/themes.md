---
title: "2. Finding and Installing a Theme"
date: 2020-11-17T13:05:56+05:30
draft: false

categories: ["Hugo"]
icon: "fas fa-fire-alt"
---

## Themes

You can browse through the themes listed at https://themes.gohugo.io/.

When I was first using hugo, I followed the [Free Code Camp Hugo Tutorial](https://www.freecodecamp.org/news/your-first-hugo-blog-a-practical-guide/), and they recommend using the Ghostwriter theme if you are starting out. We will instead pick a different design.

We will be using the Hugo-sugoi theme for now. You can read about it [here](https://themes.gohugo.io/hugo-sugoi/) and check out the demo [here](https://themes.gohugo.io/theme/hugo-sugoi/).

Download the source code from [Github](https://github.com/aanupam23/hugo-sugoi) (Click on the Green **Code** button, then **Download ZIP**).

Extract the zip, and copy the `hugo-sugoi-master` into your `my-food-blog\themes` folder. Don't forget to make sure that the folder has been extracted correctly. For example, make sure the theme's code is nested under `my-food-blog\themes\hugo-sugoi-master` and not `my-food-blog\themes\hugo-sugoi-master\hugo-sugoi-master`.

Now rename the folder from `hugo-sugoi-master` to `hugo-sugoi`.

You can run the site now without modifying it to see what it looks like, just make sure to open `my-food-blog\config.toml` and make sure you have the following code:

```
baseURL = "/"
languageCode = "en-us"
title = "Your website's name"
theme = "hugo-sugoi"
```

The HTML files are split up into **partials**. These partials only contain the HTML code for that particular section. For example, the `header.html` will only contain the HTML code for what is in the header of your website.

Go into `my-food-blog\themes\hugo-sugoi\layouts\partials\header.html`.

Change:

```
<label for="drop" class="toggle"><i class="fas fa-bars u-pull-right" aria-hidden="true"></i> 
	<span><i class="fas fa-fire" aria-hidden="true"></i> 
		Sugoi // Change Sugoi to your website's name (or, 'Home')
	</span>
</label> 

```

Also, change:

```
<li><a href="{{ .Site.BaseURL }}">
	<span><i class="fas fa-fire" aria-hidden="true"></i>
		Sugoi // Change Sugoi to your website's name (or, 'Home')
	</span>
</a></li>

```
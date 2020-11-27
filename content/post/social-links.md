---
title: "Social Links"
date: 2020-11-17T15:05:56+05:30
draft: false

categories: ["Hugo"]
icon: "fas fa-fire-alt"
---

## Social Links

Open `my-food-blog\config.toml` and overwrite the code to this (substituting your details):

```
baseURL = "/"
languageCode = "en-us"
title = "Your website's name"
theme = "hugo-sugoi"

[Params]
  herotitle = "Your website's name"
  facebook = "https://facebook.com/XXX"
  twitter = "https://twitter.com/XXX"
  youtube = "https://youtube.com/XXX"
  github = "https://github.com/XXX"
  email = "XXX@example.com"

```

If you want to exclude some of the social media, you can just delete the lines that you do not need.

Go into `my-food-blog\themes\hugo-sugoi\layouts\partials\hero.html`. To add some social media links at the top, you can make the following modifications:

```
<div class="section hero">
	<div class="container">
		<h3 class="section-heading">{{ .Site.Params.herotitle}}</h3>
		<a class="button button-primary" href="{{ .Site.Params.herolink}}">{{ .Site.Params.herolinktext}}</a>

		// Add this code block here
		<br>
		<a class="button" style="color:rgb(112, 126, 250)" href="{{ .Site.Params.facebook}}">Facebook</a>
		<a class="button" style="color:rgb(148, 217, 238)" href="{{ .Site.Params.twitter}}">Twitter</a>
		<a class="button" style="color:rgb(253, 130, 121)" href="{{ .Site.Params.youtube}}">Youtube</a>
		<a class="button" style="color:rgb(255, 251, 250)" href="{{ .Site.Params.github}}">Github</a>
		<a class="button" style="color:rgb(132, 241, 214)" href="{{ .Site.Params.email}}">Email</a>
		// -----

	</div>
</div>

```

They will use the links that you specified in the previous `my-food-blog\config.toml` file.

If you want to add more social media links at the bottom, you can - download this [zip file](../../assets/downloads/images.zip) and copy the contents into `my-food-blog\static\images`.  

Go into `my-food-blog\themes\hugo-sugoi\layouts\partials\footer.html` and copy and paste the social media links you want:

```
<footer>
	// ------------------------------------ Add social media links
	<!-- Facebook -->
	<a href="{{ .Site.Params.facebook}}"><img style="width: 30px" src="/images/facebook.png" alt="icon"></a> 
	<span style="padding:15px">

	<!-- Youtube -->
	<a href="{{ .Site.Params.youtube}}"><img style="width: 30px" src="/images/youtube.png" alt="icon"></a> 
	<span style="padding:15px">

	<!-- Twitter -->
	<a href="{{ .Site.Params.twitter}}"><img style="width: 30px" src="/images/twitter.png" alt="icon"></a> 
	<span style="padding:15px">
			
	<!-- Github -->
	<a href="{{ .Site.Params.github}}"><img style="width: 30px" src="/images/github.png" alt="icon"></a> 
	<span style="padding:15px">

	<!-- Email -->
	<a href="{{ .Site.Params.email}}"><img style="width: 30px" src="/images/gmail.png" alt="icon"></a> 
	// ------------------------------------

	<br>
	<span class="copyright">
			{{ with .Site.Copyright | default "&copy;" }} {{ . | safeHTML }} {{ now.Format "2006"}} {{ end }}
			<a href="https://github.com/aanupam23/hugo-sugoi" title="hugo-sugoi" alt="hugo-sugoi" target="_blank">Hugo-Sugoi</a>
	</span>
</footer>

```

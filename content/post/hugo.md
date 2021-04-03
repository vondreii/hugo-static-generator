---
title: "1. Hugo"
date: 2020-11-17T14:05:56+05:30
draft: false

categories: ["Hugo"]
icon: "fas fa-fire-alt"
---

## Hugo

Online platforms such as Squarespace, Wix or Wordpress are very convenient to use to customise and create your own website. Though, they can get expensive when it comes to hosting, registeration and adding premium features.
  
Hugo is a framework where you can create your own website, completely from scratch without much effort or without knowing too much (or any) of the internal programming.
There are also many web hosting platforms that can easily host a Hugo project for free - meaning, the only money you will spend will be for the custom domain name!

You can choose from lots of amazing free themes. Each blog post is written as a `.md` file, also known as `markdown`. Markdown can just be written as plain English with a few added symbols to symbolise where the headings are, which words are bold, or any other special formatting that may be needed.

### Installing Hugo

Create a folder where you want to store your project.

Go into the command prompt and navigate to the folder you have created. Run `cd <path to your project folder>`. For example, I created my folder `hugo website` in the Desktop, so I would run:

`cd C:\Users\Sharl\Desktop\hugo website`

Now, we will install hugo and create a new project from scratch. In the command prompt, we will run a few commands that will install hugo and create the base of the website.

For windows, if you use chocolatey for package management, run:

`choco install hugo -confirm`

otherwise if you use Scoop for package management, run:
`scoop install hugo`

You can check what you are using by going into your `C:\ProgramData` folder and seeing if you either have chocolatey or scoop.

To install hugo using a MAC:

`brew install hugo`

To install hugo using Linux:

`brew install hugo`

### Creating a new project

Now that we have hugo installed, we can start our project.

In the command prompt, run `hugo new site <name of blog here>`. For this example, we will make a blog about food, which will be called 'My Food Blog':

```
hugo new site my-food-blog

```

This will create a new folder called my-food-blog. If you open the folder, you will see that the 'skeleton' or 'base' folders have automatically been created.
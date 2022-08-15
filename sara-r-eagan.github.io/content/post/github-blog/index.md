---
authors:
- zc
categories:
- blog
date: "2020-08-22T00:00:00Z"
draft: false
featured: true
image:
  caption: Photo credit to [**BBVA**](https://bbvaopen4u.com/en/actualidad/best-blogs-apis)
  focal_point: ""
  placement: 2
  preview_only: false
lastmod: "2020-08-22T00:00:00Z"
projects: []
subtitle: ""
summary: A walk-through of what I did to build my blog site using GitHub Pages.
tags:
- dev
- professional development
- web development
- Git
title: Building a Website Using Git Pages
---

This method requires a basic understanding of how Git works, and how Markdown works. These aren't super complex systems, but definitely come with a little bit of a learning curve. This is a place to get started, and from here it will just take time to get a handle on everything. In the end, if you are in academia or writing, or if you are doing any remotely technical work, understanding Git and understanding Markdown will actually pay off for you bigtime in the end! I **highly** recommend this approach!

## GitHub Pages

So, the appraoch that I am pushing here is [GitHub Pages](https://pages.github.com/). Doing this, your domain is setup and your content is hosted. If you want, you can still setup your own domain name, but you don't have to (the domain will default to username.github.io). The framework that I use and will be describing is [Hugo](https://gohugo.io/). The [Hugo](https://gohugo.io/) theme that I will be describing is [Academic](https://themes.gohugo.io/academic/). The whole thing is managed by pushing to a [GitHub](https://github.com/) repository.

## Domain Name

To start, we will be discussing domain name options. As I mentioned above, using [GitHub Pages](https://pages.github.com/), you don't have to do anything to setup a domain name, but you can. Having a domain essentially means that you own a web address. For instance, my domain is [neurophysicole.com](neurophysicole.com). If you follow the link, you'll notice though that the web address changes to `neurophysicole.github.io`. This is essentially because I didn't want to bother with the process of getting that to change. I setup the domain to forward. This way, I can tell people to go to `neurophysicole.com` rather than `neurophysicole.github.io`, which is a little more ponderous (neurophysicole is already long and crazy enough!). Now, just because I am just using a forwarding address, doesn't mean you can't explicitly attach your domain to your website. I may eventually fully replace the github.io domain, but at the moment I am not really inspired to go down that rabbit hole. For more information on how to do that, check this [GitHub Pages documentation](https://docs.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site) page outlining the process.

The additional perk to having a domain is that I have an email address attached. In the past 5 or 6 years, I have been at three universities. And I plan to move on to a new one in the next few years! My email is constantly changing! So, I figure this is a good way to keep a consistent email. **Note:** I don't actually have the email setup, I have an email address attached to my domain that forwards to whatever email I am using as my primary at the time. It is so easy to setup and I feel like the payoff is totally worth it!

Setting up a domain is very easy. I only have experience doing it through one service: [Hover](https://www.hover.com/). The customer service is great, and the interface is incredibly easy to use. Setting up the additional domain name means that this is no longer a free option. The price for my domain was reasonable, and the additional price for the email forwarding was cheap, so altogether, it seems like a solid payoff for me.

## Git

So, the website is hosted on [GitHub](https://github.com/). This means that if you do not already have a [GitHub](https://github.com/) account, you need to set one up. GitHub has moved everything to free accounts, so setting up your page is totally free! Once you create an account, you need to create a repository (sometimes referred to as a 'repo') named '`your username`.github.io'. Initialize it with a README. Now, your site is up and running! ... But empty.

\* **Note:** Going from here, you kinda need to know how Git works. If you are lost with that, I would recommend looking at the resources available on [GitHub](https://github.com/) or elsewhere on the internet.

Something else we should do while we're on [GitHub](https://github.com/) is to setup another repo. You can name this one whatever you want. For example, mine is `z_site`.

Okay, now that you have the repos setup online, it is time to take advantage of the beauty of Git! Clone your repos to your computer. (This is a very basic Git process, so I am not going to explain -- but there are tons of reources on [GitHub](https://github.com/) and other great blogs I am sure..)

## RMarkdown

Now we are going to divert real quick to the [RMarkdown](https://rmarkdown.rstudio.com/) stuff, but will come back to the Git stuff right after. Order is important here, so I would just recommend following along. So, if you aren't familiar with Markdown, here is a link to the [Markdown Wikipedia page](https://en.wikipedia.org/wiki/Markdown). Essentially, it is a way to create a document without having to really worry about formatting. Additionally, it is a document type that works well for blogs. For instance, this post was written entirely in a Markdown document.

[RMarkdown](https://rmarkdown.rstudio.com/) is a form of Markdown that is built within the open-source software [R](https://www.r-project.org/). The reason we use [RMarkdown](https://rmarkdown.rstudio.com/) is because there are packages that [Academic](https://sourcethemes.com/academic/) needs to function. So, if you don't have [R](https://www.r-project.org/), or don't know how to use [R](https://www.r-project.org/), you are probably going to have a bit of a curve here, but I'll try and help.

So, if we're starting from scratch, you'll want to download [R](https://www.r-project.org/). After that, download [R Studio](https://rstudio.com/). Now, in [R Studio](https://rstudio.com/), enter the following:
- `install.packages('blogdown')` <- installs the main package that we'll be working from: [Blogdown](https://bookdown.org/yihui/blogdown/)
- In [R Studio](https://rstudio.com/), select `File` > `New Project`
  - Select `New Directory`
  - Select `Website using blogdown`
  - Name the folder you want to make your site in (I'd recommend making it the same name as your main website repo - whatever it is. e.g., `username.github.io`)
  - Create your site in the sub-directory of the `z_site` repo you made (or, whatever you decided to name it)
  - Select `Install Hugo automatically`, `Add sample blog posts`, `Add the example site of the theme`, `Convert all metadata to YAML`
  - For the Hugo theme: input `gcushen/hugo-academic`
- `library('blogdown')` <-- activates the package
- `blogdown::serve_site()` <-- activates a local server so you can see your website! Run this line whenever you want to see your changes.

Now you should see the site you are working with in the Viewer! What you are viewing is a template, but it helps to see what is there. You can choose to edit the existing content, or you can create your own content. The example site is one page, but you can add others by adding folders in your site with an `index.md` file (name the folder what you want the page to be named). If you want to have a link in the menu on the top bar of your website, update the `config` > `default` > `menus.toml`. While we're in this folder, keep in mind, the `.toml` files in this folder set the basic settings for the entire website. Feel free to explore. For more information, check [Academic](https://sourcethemes.com/academic/).

You have the freedom now to do what you want! After making a change, enter `blogdown::serve_site()` to see what it will look like!

## Hugo vs. Jekyll

Like I said earlier, I use a [Hugo](https://gohugo.io/) framework. If you look at the [GitHub Pages](https://pages.github.com/) documentation, that system is built mainly to work with a [Jekyll](https://jekyllrb.com/) framework. This makes things a little tricky, but we'll work it out here.

It is worth noting that this is the point in the development of my own site that I ran into the most issues. I had been working off of a couple of other blogs describing what they had done, and that kind of led me astray. I think in the end, whatever they did worked for them, but it was either outdated information, or I just wasn't able to replicate it for some reason. There are multiple solutions to this issue of getting the [Hugo](https://gohugo.io/) framework to play nice with [GitHub](https://github.com/), I think what I have come up with seems to work really well, and is really easy to maintain.

Now, we have to get our site online. In the file structure of your website, there is a `public` folder. [RMarkdown](https://rmarkdown.rstudio.com/) converts the .md (Markdown) files into .html (I think), and these converted files are stored in the `public` folder. This is what we need to get on your `username.github.io` repo. If we do this properly, we'll have your site up and running shortly! So, what we need to do is copy the files from the folder made when you cloned your `username.github.io` repo to your computer. There should be a README, and one or two hidden files (e.g., `.git`). The important ones are the hidden files. There is more than one way to do this. I am using a Mac, so if you are using a PC, things might be a little wonky. But I think you can set your file explorer settings to show hidden files, then you can just copy over the files. If you are using a Mac, I recommend the using the following code in the Terminal app:
- `cp -a folder_path/username.github.io_folder/.* folder_path/z_site_folder/username.github.io_Rmarkdown_website_folder/public/` <-- moves the website repo into the public folder (this is what we need for the website to work)
- `cp -a folder_path/username.github.io_folder/* folder_path/z_site_folder/username.github.io_Rmarkdown_website_folder/public/` <-- moves the README, and any other files you have created, into the public folder
- `rm -rf folder_path/username.github.io_folder` <-- removes old cloned repo - we don't need it anymore

To check that we are all good, you can check the status of your repo by entering the following lines in the Terminal app:
- `cd folder_path/username.github.io_folder` <-- moves into the secondary (`z_site`) repo folder
- `git status` <-- should bring up the files that were added to the folder
- `cd public` <-- moves into the main website repo folder (this can be kinda confusing, but it is the `username.github.io` repo)
- `git status` <-- should bring up the files that were added to this folder
  
So, as a quick recap before we go live with the website. We have created our site in [RMarkdown](https://rmarkdown.rstudio.com/), then we have moved it into the secondary repo folder (mine is called `z_site`), then we copied the files from our main repo into the `public` folder created by the website. This public folder contains the files we want in the repo that we originally setup for our website. So, this means now that we have a repo-inception where we have the secondary repo containing all of our files (`z_site`), and we have the main repo (`username.github.io`) within that repo. Although we have this repo-inception going on, we still have to update both repos. If you use a Git software, you can use that, but if you want to do it in the Terminal app, use the following code:
- `cd folder_path/username.github.io_folder` <-- moves into the secondary (`z_site`) repo folder
- `git add .` <-- adds everything to the queue to be committed
- `git commit -am "Log what you did here."` <-- compiles and commits all of the changes
- `git push origin master` <-- pushes your changes to the secondary repo
- `cd public` <-- moves into the main website repo folder
- `git add .` <-- adds everything to the queue to be committed
- `git commit -am "Log what you did here. Can be the same message as the other commit."` <-- compiles and commits all of the changes
- `git push origin master` <-- pushes your changes to the main website repo - your site should be online now!

Yay! We should be all good now! Now, just remember that in order for your changes to be expressed on the website, you have to run the following code in [RMarkdown](https://rmarkdown.rstudio.com/): `blogdown::serve_site()` so the .md files are converted to the .html files and moved into the `public` folder.

Now that we're here, I have something to share with you, and don't be mad.. but I promise the stuff we just did was the best way to go. Now, if you don't want to deal with two repos, you can just create a repo for the `public` folder, and not worry about the secondary repo. The reason I like to roll with two repos is that if anything happens with the content outside of the public folder, your whole wesbite is lost (or, at least incapable of being updated). Having that Git repo is bigtime! That is the beauty of Git! Use it!!

## Updating Your Site

You're setup now! Make it yours. Spend some time reading through the [Academic documentation](https://sourcethemes.com/academic/), get familiar with the file system and how it works. Customize the things you need for the site to be yours! Or don't, that's up to you! As part of your initial development process, I would recommend that you build templates for your posts. You will save time by just copying the files into the folder that you need, updating the YAML header, and adding in the content that you want. And I would recommend looking at the Hugo example when you are trying to figure out how to do something. At this point, it's all yours. Have fun with it. Good luck!

## Point-and-Click Using WordPress

There is so much that I just cannot cover, it really is just best to look at the relevant documentation. I think I wasted probably ~6 hours trying to get things working because I was working off of some blogs that were misleading (hopefully I don't do that to you!), so although it is nice to get the information condensed from blogs and such, it is probably best just to go straight to the source. Also, the [GitHub Pages documentation](https://pages.github.com/) and the [Hugo-Academic documentation](https://sourcethemes.com/academic/) is pretty great! If you have gotten to this point, and you think that maybe this is not the route for you to take, checkout my other blog outlining what you need to know to setup a blog site using [WordPress](https://wordpress.com/), and some advice based on what I have done in the past: [Building a Website Using WordPress](/post/wordpress-blog/).
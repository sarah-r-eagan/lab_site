---
authors:
- zc
categories:
- blog
date: "2020-08-22T00:00:00Z"
draft: false
featured: false
image:
  caption: Photo credit to [**Tech Radar**](https://www.techradar.com/news/best-blogging-platform)
  focal_point: ""
  placement: 2
  preview_only: false
lastmod: "2020-08-22T00:00:00Z"
projects: []
subtitle: Point-and-Click
summary: A walk-through of what I have done in the past to develop websites using mostly point-and-click.
tags:
- dev
- professional development
- web development
- WordPress
title: Building a Website Using WordPress
---

Despite this method requiring no real technical/programming expertise, there is still a learning curve. The following is a guide to help you through the process:

## Domain Name

First, you will have to find yourself a domain name. Obviously, go with something that is relevant, easy to remember, and hopefully easy to spell (say that again, slowly...then spell neurophysicole..haha). Something that I did learn, was that if you are able to attach your website to another highly trafficked website, your page will be more likely to show up in Google searches and such. For example, if your University offers blog space, you could create your own attached url (e.g., blogname.university.edu). The university may give some push-back if you choose to go with blogname.university.edu, and may try to push you more towards a university.edu/blogname url (saying this from experience). Either way, it is still generally recommended that you use the university resources if possible. This will save you money, and probably help with the visibility of your website.

In the end, if you are not satisfied with your domain name, you can purchase a domain and set it to forward to your university url. This way you can still advertise your website as you would like, but can save time/money/effort in setting up hosting and other things. It just makes more sense.

When purchasing a domain, there are a variety of options. I am not an expert, but in my discussions with individuals who seem to know what they are talking about, [Hover](https://www.hover.com/) has been the most highly recommended company to go through. In my experience, [Hover](https://www.hover.com/) has been great with customer support and their system is relatively simple to use (I don't have experience with other companies, so I cannot speak too much in comparison, but I have heard some negative things about other popular options).

## Hosting

Second, if you are not using an already established site (i.e., using a university or company url), you will need to setup a hosting option. This is something that I was completely unaware of going in, and I think is probably where the majority of your cost will be (often times these hosting companies offer a really cheap Year 1 price, then hike it up bigtime for Year 2, and so on). You might be asking yourself, what is hosting and why do I need it?? Well, web hosts essentially provide space on a server to hold all of the content of your website. Think of purchasing web hosting as purchasing space on a hard drive where your website will be stored. Additionally, hosts will provide tools for screening your site for viruses, provide email options, and other things (that I cannot think of off of the top of my head).

Things to consider when selecting a host are their reputation as far as how fast your website loads, and how reliable it will be (how often your site will crash). Things that matter are how much traffic you expect to have to your website, and how much information you plan to store on your site (including email). You'll have to look at the hosts themselves to know for sure how your needs will affect cost. As far as I know, there are two main differences between hosts: (1) Some provide you with your own section on a server, others offer shared space on a server. The shared server will work fine for smaller sites (personal, or maybe even for your average research lab), but they are _more_ likely to have issues as far as crashing and slowdowns are concerned; (2) Shared services are cheaper.

As far as a recommendation goes, I think the most highly rated options are [BlueHost](https://www.bluehost.com/) and [SiteGround](https://www.siteground.com/). I personally have used [SiteGround](https://www.siteground.com/), and their service was great. The user interface is admittedly not-at-all intuitive (probably the worst user interface I have ever used..). Fortunately, I did not have to check it often, but setting everything up was a little more difficult than I would have liked. Overall, I was very happy with the service, but like I have said in the past, I do not have any reference for comparison, so other options could very well be just as viable, or better/easier to use.

## Content Management

Third, you will have to make a decision regarding content management. I tend to think of this as the operating system for your website. There are numerous options, but the overwhelming majority of the internet is built on [WordPress](https://wordpress.com/). As such, it is fairly easy to find support when developing a website using [WordPress](https://wordpress.com/). I cannot speak to the other systems, but I would say if you not an experienced web-developer, and are not trying to become an expert, [WordPress](https://wordpress.com/) is probably a good way to go. Everything that I discuss from here-on-out will be within the context of a [WordPress](https://wordpress.com/) environment.

## WordPress Theme

[Wordpress](https://wordpress.com/) themes are essentially the template that you will use to build your website around (color scheme, layout, basic features, etc.). Each theme has its own preset structure, and they all vary in their additional features and support. Things to consider when choosing a theme are (of course) the layout, cost, and the support. There are free themes, and there are $$ themes. Anyone can develop a theme. As such, some random person or small group (more likely to be open source) is less likely to provide long-term support for their theme, as compared to some of the more popular options.

That being said, I believe that [Divi](https://www.elegantthemes.com/gallery/divi/) is probably the most popular theme chosen for [WordPress](https://wordpress.com/). This is not an open source theme, but is very easy to use. You do not have to know how to program (for the most part, at least), and there are a lot of options for your layout. Furthermore, [Divi](https://www.elegantthemes.com/gallery/divi/) is very well supported, and there are a lot of easy to find solutions for common problems. Finally, [Divi](https://www.elegantthemes.com/gallery/divi/) comes with a ton of built-in widgets and plugins that are often updated. If cost is not an object (at least on this level), then I would highly recommend going with [Divi](https://www.elegantthemes.com/gallery/divi/) for your website.

For my own website, I decided to try something open source (if you aren't sure what I am talking about when I mention 'open source', check out the [OpenSource website](https://opensource.com/resources/what-open-source)). After quite a bit of research, and some trial-and-error, I decided to go with [OceanWP](https://oceanwp.org/). This theme has provided me with the flexibility I needed to customize the features I am particular about, uses a GUI base (not requiring programming skills), appears to be fairly well-supported, and is compatible with a lot of great plugins!

## Plugins

Fourth, if you did not (or do not intend to) purchase [Divi](https://www.elegantthemes.com/gallery/divi/), you will probably require some plugins to get your website functioning as you would like to (I did, at least). Things to think about for plugins are generally the same as the themes. Things that plugins can be useful for are organizing your site and the working environment, and any other specialized customization you might want to attempt. The plugins that I used are [Elementor](https://elementor.com/) (for a more advanced GUI based working environment for developing the website), [Content Views](https://www.contentviewspro.com/) (to organize my blog layout), [Blog2Social](https://www.blog2social.com/en/) (to automatically share my posts to my attached social media). These will require some research on your own, depending on what you want your site to be capable of.. but I would recommend these as a starting point.

## Developing Your Site

Fifth, now you have to develop your website. This is the fun part! Anyways, as a general principle I would recommend (as it was recommended to me) to create the parts of your site that will be updated by making them blog posts (this way they can be developed in one place, organized, and added automatically). Second, work with templates! Everything will be easier, especially if you are developing a blog such as this one, if you just have a general template you work with, making minor tweaks here and there. Along these lines, I would recommend working with the layout of the site as much as possible. The more you try and change the layout, the more difficult it will be to develop and maintain. Furthermore, if you are a person that does not have a lot of undedicated free time, you are probably not going to be able to continually update your site - and if you do have the time, I'm sure it will get old at some point. The point is, once your site is developed, you are just going to want to add content. If you have to keep making adjustments, the addition of content just isn't going to happen (a) because you don't have the time, and/or (b) because you're tired of working on your site and do not want to do it. (I have experienced both).

## Using GitHub Pages

Okay, all that should get you through the basics of building your own blog site. All this said, I personally prefer to build my site using [GitHub Pages](https://pages.github.com/) and Git. For this reason, and also because [GitHub Pages](https://pages.github.com/) is an effective no-cost option, I completely re-built my website into what it is now using [GitHub Pages](https://pages.github.com/). That said, there are other point-and-click no-cost options, but the opions I came across just weren't what I wanted. This [GitHub Pages](https://pages.github.com/) option is free, and I just like it better! I am generally a "you get what you pay for" guy, but here, I think I have found a possible exception (in my case, it seems more like a "you get out what you put in" situation). To see how I re-built my website using [GitHub Pages](https://pages.github.com/), check out this blog post: [Building a Website Using Git Pages](/post/github-blog/)!

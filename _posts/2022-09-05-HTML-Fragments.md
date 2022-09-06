---
toc: true
layout: post
description: Using HTML fragments and learning about ways to format Fastpages.
categories: [markdown, week2]
image: images/Using_colors.png
title: Using HTML Fragments
---

# Changing the Fastpages Theme

The original theme of the site is minima, but I experimented with changing it to a different supported theme. It was a little confusing at first, and I realized I needed to input specific code to change the theme.

![]({{ site.baseurl }}/images/Using_new_themes.png "Using a different theme")

The boxes which are around the articles seem to not have been there(with minima), and I don't know if that was supposed to happen when changing the theme to Merlot. The preview images were very large, instead of the small ones which minima has. Also, the GitHub user button did not seem to work.
It can be seen that minima is the optimized theme for Fastpages.

# Customizing the Fastpage Site

I experimented with dark mode on the site, as well as changing the color of dark mode from black to a different color. It is a neat way to customize the site, but I think I will stick with the regular dark mode for now.

![]({{ site.baseurl }}/images/Using_colors.png "Fancy colors.")

# Time Box Fragments

I have created a time box on the [frontpage](https://muffinman1287.github.io/FirstFastPage/) describing what I have done for the week, and linked the review ticket.

# Naming and Tagging

Naming and tagging are very useful on the blog to organize material. Using the tagging feature, I have been able to organize my posts and notebooks based on the language, the subject they are for, and they week they were posted.

![]({{ site.baseurl }}/images/Using_tags.png "Tags are very helpful in finding things quickly.")

# Using the Searchbar

The search bar is also a powerful tool for this blog. It helps to find posts with keywords, but it also finds posts with certain tags. In the image, I was easily able to search for posts with the "week0" tag.

![]({{ site.baseurl }}/images/Using_search.png "The searchbar helps to find specific items.")

# Changing _config.yml

I had originally changed the config file to show the preview images, which the site did not do before. I changed `show_image: ` to `true` and this allows for a different, more interesting format.

# Using Liquid

I learned that liquid could make creating the time box easier. Liquid has the capability of "incrememnting" variables, or adding one each time the variable is called. I used code to do this in my table, which will make it easier to set up more additions every week.

![]({{ site.baseurl }}/images/Using_liquid.png "Liquid syntax is very useful.")

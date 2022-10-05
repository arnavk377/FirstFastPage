---
toc: true
layout: post
description: Deploying my Flask Repository using AWS
categories: [week6, csp]
image: images/deploy.jpeg
title: Deployment
---

![]({{ site.baseurl }}/images/deploy.jpeg)

# Curl

I was able to use curl to display the HTML of my homepage. This specific part of the curl showcases the custom card created on my Flask Repository.

![]({{ site.baseurl }}/images/curl.png "Code")

# sudo docker ps

Here are the results in the terminal from running the command "sudo docker ps".

![]({{ site.baseurl }}/images/sudops.png "SUDOOOOOOOO")

# Group Repository

Here is our group repository hosted on the IP address of the AWS instance.

![]({{ site.baseurl }}/images/nginx-taal.PNG)

Here is our group repository hosted on a custom domain through Freenom.

![]({{ site.baseurl }}/images/taalhost.png)

The link to our repository is taalsite.tk.

# Page using IP

I was able to upload my flask repository and page to the IP address associated with the EC2 instance.

![]({{ site.baseurl }}/images/workingip.png "Flask on the Web")

# Changing the page

I was also able to change something on my repository, and then push the change to the page on the IP.

Before the change:

![]({{ site.baseurl }}/images/change2.png "No alteration")

If you look closely, you will learn to "Start with Hello!"

![]({{ site.baseurl }}/images/change1.png "Hello!")

It can be seen that these are both hosted on the same IP, but the pages are clearly different. It shows how easy it is to update and change a website.

# Using a Custom Domain

Despite the problems with Freenom earlier, it began working, and I was able to use a custom domain and DNS service to host the repository.

![]({{ site.baseurl }}/images/with_link.png "Domain!")

If you look at the search bar, you can see that domain is not the IP address of the AWS instance, but a domain which I made. Here is the [link](http://arnavcspsite.tk/).

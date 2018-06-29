# Public Interest Tech Blog template

To install, fork on github and modify the `/_data/bio.yml` and the `_config.yml` file.
Use the files in `_posts` to get started in filling in your own content, and 

Demo: [https://pit.andrewlb.com](https://pit.andrewlb.com)

## Installation
* Fork the repository
* If you're working on it locally, make sure to update with the pit config by running `git submodule update --recursive --remote`
* Update the `_config.yml` file
* update the `_data/bio.yml` file with your bio.
* Go to settings and set Github Pages source as master.
* (Optional) Set up your custom domain and make sure to force HTTPS (may take a few days)
* Your new site should be ready soon, but will take time to propogate.

## Posting
* Put your posts in `_posts` in the format provided  (eg `2018-07-01-demo-post.md`)
* Make sure the top of the post has meta data.
```
---
layout: post // References template
title: "Demo Post" // Title of post
permalink: sample // This is the link, so grant-calculator = https://pit.andrewlb.com/grant-calculator 
author: Author Name // Your name
description: Here is the description // Description that goes on the home page
comments: true // Not implemented in this version, but you can add disqus
tags: [tags] // Tags for SEO
image: '/images/posts/buildplane.jpg' // path to image that appears at the top of your post + on the home page
---
```
* You can add new pages that appear in the nav bar in `_pages`. You can add links to those pages in `_includes/header.html`

## Troubleshooting
If the "other fellows" collection isn't being called, open your `.gitmodules` file and verify that this line is present. Github pages requires the https url ref for using submodules, vs. the standard remote git path.
```
[submodule "_data/_config"]
	path = _data/_config
	url = https://github.com/NewAmericaPIT/_config.git
```


### About
Built by [Andrew Lovett-Barron](https://github.com/readywater) for his [fellowship blog](https://pit.andrewlb.com).
Heavily modified with from Vyaasa as a starting point theme.
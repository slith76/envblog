---
layout: post
title: "Creating a Github Blog Using Octopress"
date: 2013-02-12 13:37
comments: true
categories: 
---
## Quick Install and Posting Sample

### Links:

* https://github.com/imathis/octopress
* HOWTO based on: http://www.tomordonez.com/blog/2012/06/04/creating-a-github-blog-using-octopress/

### Install:

	mkdir VIMLearningBlog
	git clone git://github.com/imathis/octopress.git octopress
	cd octopress; bundle install
	rake install

on github: create new repo #envblog
GITURL: git@github.com:slith76/envblog.git

	rake setup_github_pages
	git remote -v
	git remote add origin git@github.com:slith76/envblog.git
	git branch
	git branch -m master source
	rake preview #http://127.0.0.1:4000/envblog/

### First push to github:

	rake generate
	git add .
	git commit -am "First deploy to github."
	git push origin source
	rake deploy
### Create a new Posting:

	rake new_post["Creating a Github Blog Using Octopress"]
	cd source/_posts/; #edit Posting
	rake generate
	git add .
	git commit -m "Initial blog post."
	git push origin source
	rake deploy

### Install a new Theme:

	git clone git://github.com/tommy351/Octopress-Theme-Slash.git .themes/slash
	rake install['slash']
	rake generate && git add . && git commit -m "Post Update" && git push origin source && rake deploy

#### Themes can be found under:
http://octopressthemes.com
https://github.com/imathis/octopress/wiki/3rd-Party-Octopress-Themes 

URL: http://slith76.github.com/envblog/

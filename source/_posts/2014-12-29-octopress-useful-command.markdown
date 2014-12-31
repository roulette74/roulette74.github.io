---
layout: post
title: "octopress useful command"
date: 2014-12-29 21:00:37 +0800
comments: true
sharing: true
categories: 
---
Setup Octopress:

    > git clone git://github.com/imathis/octopress.git octopress
    > cd octopress
    > gem install bundler
    > rbenv rehash # If you use rbenv, rehash to be able to run the bundle command
    > bunde install
    > rake install
    > # create a new github repository called <username>.github.io
    > rake setup_github_pages
    > > git@github.com:<username>/<username>.github.io.git
    > 
Generate new post(The markdown fill will be created at source/_posts):

    > rake new_post["octopress useful command"]
    > rake new_page[super-awesome/page.html]

Generate content:

    > rake generate

Preview content:

    > rake preview

Deploy your blog content (first deploy require around 30 minutes to create on <username>.github.io):

    > rake deploy

Don't forget to push your source code:

    > git add.
    > git commit -m 'commit message'
    > git push origin source



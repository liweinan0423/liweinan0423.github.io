---
layout: post
title: 'Building a Blog With jekyll'
date: '2015-08-28 16:24'
---

# Building a Blog with Jekyll

This is acutally my first technology blog, born faster thant I expected :)

I would like to write down some instructions on how to setup a personal blog system with [Jekyll](http://jekyllrb.com/), which is a static website generating tool written with Ruby.

Here I am just recording my own ideas on using `Jekyll`, you may find the comprehensive Jekyll guide on its [office website](http://jekyllrb.com/).

# How to Install Jekyll

Jekyll is distributed as a Ruby Gem. Hence obviously you can install it by simply typing `gem install jekyll`.

# Creating a Blog Site Project

Under any directory, execute `jekyll new myblog` will generate a folder named `myblog`, that contains all essential files for your blog website.

`cd` into the `myblog` folder, you will see the following layout:
<pre>
`--myblog
  `--_config.yml
  `--_includes/
  `--_layouts/
  `--_posts/
</pre>
I would not introduce what each folder contains except the `_posts` folder, you can find detailed explanation at [here](http://jekyllrb.com/docs/structure/).

The `_posts` folder contains plan text files, each text files is a post in your blog. It's very easy to start writing a post  by creating a text file in this folder. But be caution, the name of the text file must be in the following format:

    YYYY-MM-DD-title.FORMAT

`YYYY` is a 4 digits number represents the `Year`; `MM` and `DD` is 2 digits number represents `Month` and `Day` accordingly; `TITLE` is the title is your post; `FORMAT` is the format in which you would like to write your post. Jekyll supports `markdown` and `texttile` out of the box, and I prefer the `markdown` format.

After you finish your fist post file, `cd` to the root folder of your blog project and type

    jekyll serve

In several seconds you will see a message on the console like this:
    Server address: http://127.0.0.1:4000/
    Server running... press ctrl-c to stop.

Then open your favorite browser and go to `http://localhost:4000` and you will see your first blog up and running!

![Jekyll Started Up](//{{site.url}}/assets/images/jekyll-startup.jpg)


TO BE CONTINUED...

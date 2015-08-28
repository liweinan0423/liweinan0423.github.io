---
layout: post
title: 'Building a Blog With jekyll'
date: '2015-08-28 16:24'
---

# Building a Blog Website with Jekyll 使用Jekyll创建博客网站

This is acutally my first technology blog, born faster thant I expected :)

这就是我的第一篇技术博客了，诞生的比我预计的要早一些。 :)

I would like to write down some instructions on how to setup a personal blog system with [Jekyll](http://jekyllrb.com/), which is a static website generating tool written with Ruby.

我想记录一下如何使用Jekyll（一个使用ruby开发的静态网站生成工具）建立一个个人博客网站。

Here I am just recording my own ideas on using `Jekyll`, you may find the comprehensive Jekyll guide on its [office website](http://jekyllrb.com/).

在本篇文章中，我只是想简单的记录一下我自己所总结出的关于Jekyll的一些用法。可以去Jekyll的官方网站中寻找更全面的指南文档。


# How to Install Jekyll 如何安装Jekyll

Jekyll is distributed as a Ruby Gem, So the installation becomes very easy that you can install it just by simply typing `gem install jekyll`.
Jekyll 是一个Ruby Gem。所以安装变得很简单，只需要输入 `gem install jekyll`

# Creating a Blog Site Project 创建一个博客工程

Under any directory, execute `jekyll new myblog` will generate a folder named `myblog`, that contains all essential files for your blog website.
在任何目录下，运行`jekyll new myblog`自动创建一个名为`myblog`的目录(当然你可以给它起任何的名字)，你的博客网站所需要的所有基础文件都被包含在这个目录中。

`cd` into the `myblog` folder, you will see the following layout:
进入这个目录，可以看到如下的目录结构
<pre>
`--myblog
  `--_config.yml
  `--_includes/
  `--_layouts/
  `--_posts/
</pre>
I would not introduce what each folder contains except the `_posts` folder, you can find detailed explanation at [here](http://jekyllrb.com/docs/structure/).
除了`_posts`目录，其他的目录笔者就不详细介绍了，可以在[这里](http://jekyllrb.com/docs/structure/)查看

The `_posts` folder contains plan text files, each text files is a post in your blog. It's very easy to start writing a post  by creating a text file in this folder. But be caution, the name of the text file must be in the following format:
`_posts`目录中包含的都是文本文件，每个文本文件就是一片博客。创建了一个文本文件，也就意味这创建了一片博客，很简单。但是请注意，这个文本文件的名字必须符合以下格式：

    YYYY-MM-DD-title.FORMAT

`YYYY` is a 4 digits number represents the `Year`; `MM` and `DD` is 2 digits number represents `Month` and `Day` accordingly; `TITLE` is the title is your post; `FORMAT` is the format in which you would like to write your post. Jekyll supports `markdown` and `texttile` as well as HTML out of the box, and I prefer the `markdown` format.
其中，`YYYY`代表四位数的年份；`MM`和`DD`分别代表2位数的月份和日期；`TITLE`是这篇博客的标题；`FORMAT`是博客的格式。Jekyll支持`markdow`和`texttile`等格式，当然HTML也是支持的。作为一个程序员，我个人偏向于使用markdown格式

# Get Your Blog Website Up and Running 启动博客网站

After you finish your fist post file, `cd` to the root folder of your blog project and type
当你完成了第一篇博客的编辑之后，进入到工程的根目录，然后输入

    jekyll serve

In several seconds you will see a message on the console like this:
几秒钟之后，你会看到类似下面的信息
    Server address: http://127.0.0.1:4000/
    Server running... press ctrl-c to stop.

Then open your favorite browser and go to `http://localhost:4000` and you will see your first blog up and running!
然后打开你的浏览器，跳转至 `http://localhost:4000`，你应该就可以看到博客网站已经在运行啦！
![Jekyll Started Up](//{{site.url}}/assets/images/jekyll-startup.jpg)


TO BE CONTINUED...

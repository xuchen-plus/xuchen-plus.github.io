---
layout: post
category : random thoughts
tagline: "just a test"
tags : [intro, beginner]
---
#####在windows 7上搭建了一下jekyll，本地调试博客比较方便些，省的一遍遍push到github上。主要是安装ruby和devkit。
- 安装ruby193:
	+ [http://rubyinstaller.org/downloads](http://rubyinstaller.org/downloads)
	+ 注意：不要安装到**带空格**的目录下！！
- 安装devkit，同上面的链接，注意要和ruby安装包对应上
- 初始化devkit：
{% highlight bash %}
cd /path/to/devkit
ruby dk.rb init
ruby dk.rb install
{% endhighlight %}

- 更换taobao gem源：gem源是放在S3上的，国内访问太慢了，换成淘宝的：
{% highlight bash %}
gem sources --remove http://rubygems.org/
gem sources -a http://ruby.taobao.org/
{% endhighlight %}

- 安装jekyll，会编译一些库，要等会儿：
{% highlight bash %}
	gem install jekyll -V
{% endhighlight %}

- 安装markdown rdiscount：
{% highlight bash %}
	gem install rdiscount -V
{% endhighlight %}

- 进入jekyll博客所在目录，执行
{% highlight bash %}
	jekyll serve  （出错的话可以加--trace看call stack）
{% endhighlight %}

- 设置中文编码：之前很多人的做法是改convertible.rb代码，现在jekyll最新版已经有解决方案，在站点_config.yml里加上一行即可。参见jekyll github pull #1449
{% highlight bash %}
	encoding: UTF-8
{% endhighlight %}

<!--more-->
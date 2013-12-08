---
layout: post
category : random thoughts
tagline: "Firefox rules"
tags : [Firefox, Chrome, Software]
---

###我为什么还在使用Firefox？
最近一段时间，公司N多个内部页面都只支持Chrome，或者就是对Firefox支持不好。当然可以理解前端同学做浏览器兼容的辛苦，但是Firefox这种江河日下的感觉还是令我感到有些伤感。我之前也多次尝试过转向Chrome，最终还是回到Firefox。今天写篇文章说说为什么我还在用Firefox，不为掀起论战，不是软文，就是纯粹个人想法。

####启动速度
很多人一提到Firefox，第一反应就是：启动慢。其实从Firefox 4开始，启动速度就不再是什么问题。我自己感觉，在不装任何插件的情况下，Firefox和Chrome启动速度基本相同。在装了差不多同样数量的插件后，Firefox启动明显比Chrome快（机械硬盘）。

Chrome新版的新标签页加载特别慢（大中华局域网问题），虽然可以禁用，但还是感觉Firefox的简洁深得我心。

####字体渲染
用Chrome最不能忍受的就是在Windows 7下悲剧的字体渲染。Firefox用的是Direct Write，而Chrome还在用已经过时的GDI，中英文字体渲染差距都很明显。另外，虽然Firefox和Chrome都可以装宋体转雅黑插件，但是Chrome下还是经常遇到某些页面上的中文无法转成雅黑，看着粗糙的宋体眼睛生疼。可能有的人会说装个MacType，但是既然Win7本身支持，为什么不用呢？

####内存占用
如果机器内存在8G以上，Chrome的内存占用自然不是什么问题。但是如果是4G以下的机器，Firefox的优势还是很明显的。开了20多个标签后，占内存差不多就Chrome的一半。另外Chrome开的标签多了后，很明显切换标签比较卡，主要原因是各个页面进程要和UI主进程通过IPC通信，子进程多了后性能瓶颈就凸显出来了。当然了，Firefox这种单进程模式就是容易被单个页面搞挂整个进程，sigh。。。现在Firefox也[计划改为多进程模式](http://billmccloskey.wordpress.com/2013/12/05/multiprocess-firefox/)，希望能比Chrome有所突破。

####网页渲染和JS
现在各种HTML 5和JS的Benchmark，Firefox都丝毫不弱。实际使用中我的感觉是，Firefox是比Chrome慢一些，但是区别不明显。更多的时候是前端优化的问题。比如前一阵天猫新首页，Firefox拖动就很卡，但是过了一段就正常了，应该是前端同学优化的结果。感觉现在前端工程师基本上都是重点保证Chrome下没问题，毕竟国内各种第三方浏览器都是Chromium内核，而Firefox还是比较小众一点。但是Firefox对HTML 5标准的支持一点不差，最新的WebSocket神马的都能支持，没有理由抛弃Firefox吧。

####标签分组
这个Chrome不知道有没有对应插件，但是Firefox原生带了这个功能。各位回忆一下有没有出现过这样一种情形：工作中开了很多很多页面，各种搜索结果，来回切换几次后一个明明记得打开过的网页标签找不着在哪了。。。用了Firefox这个功能，不同类别的标签分组管理，一下清爽了很多有木有。我的一个用法是要搜索某个问题的时候就开个新组，然后这个组内都是当前相关的页面。多个组之间可以来回切换，都看完了可以一键全部关闭。提高效率的利器。

####插件
说完浏览器本身，该说插件了。Firefox插件能做的事要比Chrome强很多，部分原因可能是Chrome为了安全考虑，很多功能都不开放给第三方插件。就说关闭最后一个标签不关闭窗口吧，这个Firefox随便一个标签管理插件都能支持，并且是真的不会关，无论是点标签上的叉还是按Ctrl-W. Chrome某些插件说是支持，其实点叉还是关了整个窗口。。。

说几个Firefox下明显比Chrome好用的插件：TabMix Plus: 这个用过的就知道了，真心超越Chrome N条街。不关窗口、收藏夹在新标签打开、搜索结果新标签打开、历史记录等等等等，不解释了。

AutoProxy或者FoxyProxy，切换代理、添加URL，都比Chrome下的SwitchySharp强太多了，尤其是AutoProxy的Proxyable item，当一个网页显示不太正常的时候，很有可能是某个资源文件的域名“挂了”，这时候用这个菜单看看，右键一点就能添加代理，上网顿时科学了很多有木有！

FireGuestures: 手势插件，在所有页面上都能用。而Chrome下类似插件，在Chrome自身的页面，例如设置、错误页面都禁用了，实际使用还是明显感觉到不方便。

Easy DragToGo+: 拖动插件。Chrome下也有，但是Firefox这个拖动链接和文字比Chrome下顺畅许多，各类JS触发的链接也都能拖，一个字：强。

其它的插件，如MultiFox、DownThemAll，以及码农必备的FireBug、ModifyHeader等等，都是相当强大的插件，就不一一列举了。

现在总体上的感觉是各种插件Firefox有点越来越跟不上节奏的感觉，很多新的应用，或者新的版本，比如Evernote、Any.DO都会先发Chrome版甚至就没有Firefox版。Firefox现在插件开发者活跃度也下降了很多，希望Firefox能重视这个问题，毕竟现在也在推Firefox OS，失去了开发者生态链，后果Mozilla应该也是知道的。

####总结
从当年的MyIE、Maxthon到搜狗，直到08年才知道了Firefox，马上为其强大的定制性所倾倒，基本上能想到的功能都有插件能实现。08年暑假Chrome第一版出来也就尝试过，一直到现在，总是觉得不如Firefox顺手。Firefox也有这样那样的问题，尤其要吐槽Flash的兼容性，但是毕竟都是小问题。
推荐台湾著名博客**[電腦玩物](http://www.playpcesor.com/)**一篇文章：
[Chrome 皮 Firefox 骨：讓人再次愛上火狐的漂亮流暢新介面](http://www.playpcesor.com/2013/11/chrome-firefox.html)




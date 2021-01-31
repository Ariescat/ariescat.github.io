> “🙉🙉🙉 ”


## 前言

Ariescat 的 Blog 就这么开通了。

本来打算在年前完成 Blog 的搭建，不曾料想踩了很多坑。。。

[跳过废话，直接看技术实现 ](#build) 

2019 年，Ariescat Blog 总算是搭建好了。

最开始写博客是在[CSDN](https://blog.csdn.net/PingXiaoGai)这个平台上，CSDN确实不错，支持markdown在线编辑。

在一次偶然间，发现了 GitHub Pages 这种神奇的存在，觉得作为一个程序员，是应该倒腾倒腾自己的Blog，于是乎就开始了撸起袖子干了。

<p id = "build"></p>

## 正文

接下来说说搭建这个博客的技术细节。  

正好之前就有关注过 [GitHub Pages](https://pages.github.com/) + [Jekyll](http://jekyllrb.com/) 快速 Building Blog 的技术方案，非常轻松时尚。

其优点非常明显：

* **Markdown** 带来的优雅写作体验
* 非常熟悉的 Git workflow ，**Git Commit 即 Blog Post**
* 利用 GitHub Pages 的域名和免费无限空间，不用自己折腾主机
	* 如果需要自定义域名，也只需要简单改改 DNS 加个 CNAME 就好了 
* Jekyll 的自定制非常容易，基本就是个模版引擎



---

其实过程也并不是很顺利，中间我还了解过 [Hexo](https://hexo.io/zh-cn/) 和 [VuePress](http://caibaojian.com/vuepress/guide/) 这两种技术。Hexo提供的中文文档非常友好，而且环境只需要node.js就好(相比起Jekyll需要ruby环境)，我不一会就把博客搭建起来了，还选了一款个人很喜欢的主题[大道至简——Hexo简洁主题推荐](https://www.haomwei.com/technology/maupassant-hexo.html)。然而每当我发布到GitHub的时候，总有一封煞笔邮件发过来，说：
> You are attempting to use a Jekyll theme, "maupassant", which is not supported by GitHub Pages.

这个问题我试了很多方法，并没有很好地解决，最终无奈放弃，选择了常用的Jekyll。

在Jekyll的搭建上，主题我直接 Downlosd 了 [Hux的博客主题](https://huangxuan.me/) 的进行修改，简单粗暴，不过遇到了很多坑😂，好在这些坑最后都填完了。。。

比如CNAME文件，绑定自己的域名的时候，这煞笔邮件又发过来了，说
> Your CNAME file was ignored because this repository is automatically hosted from Ariescat.github.io already. 

Jekyll的[安装](https://segmentfault.com/a/1190000010195733)。本地调试环境需要 `gem install jekyll`，结果 rubygem 的源居然被墙了，~~后来手动改成了我大淘宝的镜像源才成功~~，淘宝的源已经[停止维护](https://ruby.taobao.org/)，换成了OSChina的源 `https://gems.ruby-china.com/`。


## 后记

如果你恰好逛到了这里，希望你也能喜欢这个博客主题，感兴趣的话可以自己动手搭建一个。

最后，列举一些搭建博客的干货：

* [如果给你40分钟，可以搭建一个如下图所示的网站，你愿意吗？](https://blog.csdn.net/superjimmy/article/details/51626842)

* Jekyll [基本用法](https://www.jekyll.com.cn/docs/usage/)

* [Github+Jekyll 搭建个人网站详细教程](https://www.jianshu.com/p/9f71e260925d)

* Hexo [中文手册](https://hexo.io/zh-cn/)

* Hexo已经看腻了，来手把手教你使用[VuePress](https://www.jb51.net/article/138946.htm)搭建个人博客

* qiubaiying 提供的的 [Blog 主题](https://github.com/qiubaiying/qiubaiying.github.io)

—— Ariescat 后记于 2019.1



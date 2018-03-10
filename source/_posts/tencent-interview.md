---
title: 腾讯微信事业部面试
date: 2018-03-09 23:15:22
tags:
---



感谢帮忙内推的ppj还有他同学！。

### 一面

---

主要问了项目经历，项目中比较困难的地方，怎么解决的。

还问了一个跨域问题，怎么解决，原理是啥。

问了Labrador，他是怎么实现的

问了TCP，丢包，阻塞怎么解决。我印象只记得滑窗和重发

<!--more-->

最主要的是一题算法题：

> 微信小程序团队一共有 n 名成员，决定出去秋游，在海边遇到出租摩托艇的杰克马，马先生手上有 m 辆待出租的摩托艇，价格分别是 b1 、b2 ... bm;
> 由于习惯了微信支付，团队中每个人身上的现金都有限，分别是 a1 a2 ... an，对了，一起出门的老板还带有 S 元的团队经费，这个经费是每个人都可以使用的;(m>n)
>
> 那么考虑以下两个场景
>

场景1
团队成员都很有爱，都愿意借钱给其他同事，那么这时候团队最多能租到多少摩托艇

> 解法应该是把所有钱拿出来，然后直接贪心买

场景2
团队成员都十分小气，是不愿意借钱给别人的,那么请考虑以下两个问题

问题一 请判断团队成员是否都能租到摩托艇

> 这题应该是下一题的特例，即最多能租到n辆

问题二 请问给出一个策略使得整个团队租到最多的摩托艇

> 这题思路很巧妙，一开始想偏了，从小到大贪心，结果自己把自己给hack了。然后又想着能不能匈牙利求最大匹配，但是一直卡在一个S怎么分配的问题上。最后面试官提醒了，假设可以买X辆，那肯定是最有钱的X人买最便宜的X辆，然后根据这个去贪心，求最大的X。最后PBB提醒一下，这个X可以二分来求，因为是单调的。

一面总结：面试官很nice，给思考问题的时间挺充足的，会引导你去思考问题，挺棒的。

### 二面

---

首先问了一下有没有接触框架，然后我答了接触了react和vue

然后问了react和vue两者的差别

然后具体讲一下react给开发者带来了什么好处，优点。

为什么要用react不用jQuery。

答了个react提高了性能（不知道哪里看到的。。肯定是歪了。

然后面试官问react性能会比原生好？具体体现在哪里？

搜到一篇知乎

[网上都说操作真实 DOM 慢，但测试结果却比 React 更快，为什么？](https://www.zhihu.com/question/31809713/answer/53544875)

看了一下日期都是16年的了，，我真是菜啊。。

问了diff原理，我只说按层比较，紧张得语无伦次。。

然后同样的，问跨域。

跨域怎么解决，方法。

为什么浏览器要有跨域请求？

答偏了答到了XSS，问了XSS怎么预防。

然后跨域答了JSONP

问了为什么浏览器对请求有同源策略，然而对脚本没有同源策略。

也就是说为什么请求脚本可以跨域，而发送ajax请求不能跨域？

没答上来。。。

问了webpack给我们带来了什么好处？

二面总结：我觉得我答得很不好，主要原因可能缺乏思考，没有深究其原因，面试官也挺不错的，会引导你思考，一直问还有吗，还有吗，主要是想让你思维不要那么局限吧。这次面试学到了学到了，佩服佩服。Tencent的人果然都很强。



关于浏览器跨域请求我觉得需要深入学习，
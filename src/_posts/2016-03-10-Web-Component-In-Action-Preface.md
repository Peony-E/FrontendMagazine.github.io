---
layout:     post
title:      "《Web Component 实战》译者序"
subtitle:   ""
date:       2016-03-10
author:     "范洪春"
header-img: "/images/Web-Component-In-Action-Preface.jpg"
tags:
    - Web Component
    - React
    - Polymer
---

> “创建一个大型应用的秘诀就是不去创建大型应用，而把应用切分成组件。然后组装测试，由多个组件组合而成一个应用” -- JavaScriptMVC 作者，Justin Meyer

JavaScript 是一门松散类型的动态语言，在规范不够完善、社区不够健全的蛮荒时代，开发者们写出的代码也是参差不齐，没有既定规范的代码可读性差，而软件工程所提倡的复用性、可维护性、可扩展性就更是无从谈起。很难说是技术推动了产品的发展，还是快速变化的互联网带来了前端技术的进步。不过最终的结果是前端技术以惊人的速度进行迭代。正如在 JSConf 2015 开发者大会上流行起来的前端摩尔定律：“每18个月~24个月，前端都会难一倍”。前端模块化方案从无到有，从稍有模式的命名空间到 JavaScript 中的 AMD、CommonJS 模块定义，从浏览器端模块化方案再到依赖编译的 webpack、browserify 构建工具。这一路走来，毫无疑问开源社区的贡献巨大，很多新的标准也应运而生。不得不说 ES6 的模块系统很大程度上受到了 Node.js 模块的启发，HTML5 Web API 所引入的 querySelectorAll 也一定是在 jQuery 选择器中获得了灵感。

而 Web Component 则带来了 UI 组件化的全新标准。它能够帮助开发者在开发过程中创建出稳定且可复用的组件。Web Component包括模板元素、HTML Import、Shadow DOM 以及自定义元素。模板元素包含了 HTML、CSS 和 JS，可以取代传统的字符创模板；HTML Import 则可以将外部的 HTML 文档引入到当前页面中，实现了复用；Shadow DOM 则提供了样式和脚本的作用域，是 Web Component 中重要的一环；而自定义元素则可以达到扩充 HTML 元素的目的，意味着开发好一个元素后，处处可用。Web Component 做到了分离关注点，降低了代码的维护成本并且提升了开发效率，可以说是 Web 前端发展的必由之路。

值得注意的是，就现在而言 Web Component 还是一门新技术，很多浏览器都没有原生实现它。而很多走在前面的公司也以自己的方式实现了这套新标准，其中包括 Google 实现的 PolymerJS、Mozilla 实现的 X-Tag 以及 Facebook 实现的 React。它们或通过 polyfill 实现标准，或通过 Virtual DOM 另辟蹊径，这三种实现都会在本书中做详细的介绍，同样也包括了每个框架的周边类库以及构建工具，并且附有详细的代码示例。目前来看，不得不说 React 正大放异彩，国内外基于 React 搭建的项目犹如雨后春笋般崛起，这很大程度上得益于它所提出的 UI 状态机、Virtual DOM 以及单向数据流。当然，其他两个框架的设计巧思和理念同样值得每位开发者学习。

在本书中，作者详细介绍了 Web Component 的每个细节，并且通过实例深入浅出地讲解了三个基于 Web Component 规范的前端框架及其构建工具。相信读者在读完本书后一定会有所收获，能够开发自己的 Web Component 项目，或者将其思想用到现有的项目中。本书的翻译团队由4位一线 Web 开发者组成：


- **范洪春**，就职于阿里巴巴数据技术及产品事业部，前端架构方向
- **邵锋**，就职于 Splunk 中国研发中心，目前从事大数据可视化方向的开发和研究
- **何语萱**，就职于腾讯 ISUX，任 UI 工程师
- **姜天意**，就职于阿里巴巴国际事业部，主要从事 Node.js 服务端研发工作

此外，我、语萱和天意同时是知乎专栏《前端外刊评论》的维护者，本书的试读章节也会在第一时间发布到该专栏。也就意味着你在阅读本书时遇到翻译上的任何问题都可以通过专栏与我们取得联系。

最后，感谢博文视点引进了这本书，并给予我们翻译的机会。感谢 **Sandeep Kumar Patel** 创作了这本书，让更多的开发者了解这个新标准。感谢我们4个人在这段时间的相互帮助和鼓励。感谢博文视点的编辑对我们信任。感谢我在阿里的两个前端团队的同事在我负责翻译本书期间对我的理解和支持。父母之恩，毋须赘言！

<p style="text-align:right">范洪春 2015.10 于杭州</p>

## 封底

Web Component 是一个令所有开发者都激动人心的新标准，它通过封装和扩展 HTML 和 CSS 实现了可重用的强大组件。Web Component 的时代很快就要到来，并且会在你的浏览器上首次亮相。

本书以 Web Component 核心概念开篇，你可以按照书中的示例完成一个数显时钟的开发。在掌握了 Shadow DOM、HTML Import 以及模板元素的概念后，你将能够使用纯 JavaScript 创建一个自己的组件。而后，你将探索到用于开发 Web Component 的核心工具和类库，包括 Polymer、Bosonic、Mozilla Brick 以及 ReactJS，并且学会在实际项目中灵活运用它们。本书对所有架构和配置都做了详细的解释，并且选择合适的开发工具供读者学习使用。

### 面向读者

本书适合于所有想要使用新工具和技术创建 Web Component 的 Web 开发者。

### 你将从本书学到哪些

- 使用原生 JavaScript 创建 Web Component 的实战经验
- 发现 Polymer 的核心并且使用它打造你的 Web Component
- 使用 Mozilla 创建自定义的 Web Component
- 使用 ReactJS 创建别样的 Web Component
- 使用恰当的方式来创建 Web Component
- 掌握 Bosonic 框架，设计 Web Component

> 附言：本书正在热销中，适合初学者，[亚马逊](http://www.amazon.cn/Web-Component%E5%AE%9E%E6%88%98-%E6%8E%A2%E7%B4%A2PolymerJS-Mozilla-Brick-Bosonic%E4%B8%8EReactJS%E6%A1%86%E6%9E%B6-%E6%A1%91%E8%BF%AA%E6%99%AE%C2%B7%E5%BA%93%E9%A9%AC%E5%B0%94%C2%B7%E5%B8%95%E7%89%B9%E5%B0%94/dp/B017BVR54Y/ref=pd_bxgy_14_2?ie=UTF8&refRID=031SN9DEPA9YQF6927VP)、[天猫](https://list.tmall.com/search_product.htm?q=web+component&type=p&vmarket=&spm=875.7789098.a2227oh.d100&from=mallfp..pc_1_searchbutton)、[京东](http://search.jd.com/Search?keyword=web%20component&enc=utf-8&suggest=1.def.0&wq=web%20compo&pvid=pr1yfmli.umyaj1)等均有售！

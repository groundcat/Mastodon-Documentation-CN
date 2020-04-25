---
title: 什么是长毛象？
description: 欢迎来到长毛象的文档！
menu:
  docs:
    weight: -99
---

{{< youtube id="IPSbNdBmWKE" caption="An introductory video explaining basic Mastodon concepts with visual animations" >}}

## 什么是微博？ {#microblogging}

类似于发布博客，**微博**是发布小段更新到你的个人资料信息流的一种方式。您可以发布文本帖子，也可以附加图片、音频、视频或投票等媒体。长毛象让你关注朋友并发现新的朋友。

## 什么是联邦？ {#federation}

**联邦**是去中心化的一种形式。在联邦中，所有人不是都使用一个中心服务，而是使用多个任何数量的人都可以使用的服务。

| 中心化等级 | 例子 |
| :--- | :--- |
| 中心化 | Twitter, Facebook, Instagram |
| 联邦 | Email, XMPP, phone networks, physical mail |
| 分布式 | BitTorrent, IPFS, Scuttlebutt |

长毛象网站可以独立运作。就像一个传统的网站，人们在上面注册、发布消息、上传图片、互相聊天。与传统网站*不同*，长毛象网站之间可以互动，让用户互相交流，就像你可以从你的Gmail帐户发送电子邮件给某人从Outlook、Fastmail、Protonmail，或任何其他电子邮件供应商。只要你知道他们的电子邮件地址，**你可以对任何人在任何网站上的地址进行“@”或私信**。

{{< figure src="/assets/image%20%289%29.png" caption="From left to right: Centralized, Federated, Distributed" >}}



## ActivityPub是什么？ {#fediverse}

长毛象使用一种标准化的、开放的协议来实现站点之间的互动。它叫做ActivityPub。任何通过ActivityPub实现联合的软件都可以与长毛象无缝通信，就像长毛象网站之间的通信一样。

**联邦宇宙**是所有可以通过ActivityPub和万维网互相交流的网站的名字。这包括所有乳齿象服务器，但也有其他实现:

* Pleroma, 一个模块化的微博引擎,
* Pixelfed, 分享和阅读媒体文章,
* Misskey, 包括微博和可定制的仪表盘,
* PeerTube, 可以让你上传视频到频道,
* Plume, 它可以用来发布长篇文章,
*  还有更多，包括许多个人网站！

**联邦宇宙**没有自己的品牌，所以你可能更常听到“来关注我的长毛象”而不是“来关注我的联邦宇宙”，但从技术上讲后者更正确。

## 实际意义 {#implications}

### 自由选择服务提供者和用户政策{#choice}

因为长毛象是一个简单的软件，可以用于任何网站，长毛象的潜在用户可以选择从现有的长毛象网站选择服务提供商，或如果他们愿意的话，可以创建自己的长毛象网站。长毛象项目在joinmastodon.org上维护一个推荐服务提供者的列表，可按类别和/或语言进行分类。一些网站可能有特定的管理政策，比如要求使用特定的标签覆盖可能敏感的内容，一些网站可能有更宽松的政策，但网站选择器中列出所有的网站都需要同意采用长毛象服务器公约，这意味着他们承诺积极处理并反对仇恨言论、采取每日备份、至少有一个应急管理、并提供至少3个月预先通知的情况下关闭。

> 维护所有成员都感到安全的社区并不容易。长毛象提供了许多基本的框架和工具，并将权力从一个商业实体转移到社区本身。
>
> -- Eugen Rochko, Jul 6 2018, ["Cage the Mastodon"](https://blog.joinmastodon.org/2018/07/cage-the-mastodon/)

> 一个集中式的社交媒体平台有一个层次结构，其中它们的规则和实施、以及平台的发展和方向，都是由CEO决定的……
>
> -- Eugen Rochko, Dec 30 2018, ["Why does decentralization matter?"](https://blog.joinmastodon.org/2018/12/why-does-decentralization-matter/)

### 资金和盈利{#monetization}

长毛象网站是由不同的人或组织完全独立运作的，没有在软件中实现任何盈利策略。

一些服务器的运营者选择自费运营、一些运营者可以利用现有的基础设施、一些运营者依靠从他们的用户通过Patreon和类似的服务集资、一些运营者只是为自己和一些朋友搭建自费的服务器。所以，如果你想支持你的服务器的运营者，记得看看它是否提供了一个捐赠的方式。

乳齿象的发展同样是通过Patreon和OpenCollective众筹的。**不涉及风险投资**。

> 在我看来，“即时、公开、全球信息和对话”实际上应该是全球性的。在独立组织和能够自我管理的行动者之间进行分配。这是一家公共事业公司，没有利用这些对话牟利的动机。
>
> -- Eugen Rochko, Mar 3 2018, ["Twitter is not a public utility"](https://blog.joinmastodon.org/2018/03/twitter-is-not-a-public-utility/)

### 不同软件之间的互操作性{#interoperability}

在实际中：想象一下，如果你可以从你的Twitter账户关注一个Instagram用户，并在不离开你的账户的情况下评论他们的照片。如果Twitter和Instagram是使用相同协议的联合服务，这是可能的。有了长毛象帐户，你可以与任何其他兼容的网站交流，即使它不是在长毛象上运行。所需要的是软件支持ActivityPub协议的相同子集，该子集允许创建状态更新并与之交互。要了解更多有关与长毛象互操作所需的技术规范，请参阅ActivityPub、WebFinger和Security。要了解更多关于ActivityPub允许我们做什么，请看为什么ActivityPub是未来。

> 所有这些平台都是不同的，它们关注不同的需求。然而，基础都是一样的：一些人订阅另一些人的帖子。因此，它们都是兼容的。
>
> -- Eugen Rochko, Jun 27 2018, ["Why ActivityPub is the future"](https://blog.joinmastodon.org/2018/06/why-activitypub-is-the-future/)

### 免费/自由软件{#libre}

与专有服务不同的是，**任何人都可以完全自由地运行、检查、检查、复制、修改、分发和重用Mastodon源代码，前提是他们为任何派生版本赋予相同的自由度。**就像长毛象用户可以选择他们的服务提供者一样，你作为一个个体可以自由地向长毛象贡献功能，或者发布包含不同功能的修改版本。这些修改后的版本，也被称为软件分支，也需要像最初的长毛象项目一样维护同样的自由。例如，glitch-soc是一个添加了各种实验特性的软件发行版。也存在许多独立的fork，它们的主题可能略有不同，或者包含对代码库的小修改。因为乳齿象是自由软件，尊重你的自由，像这样的个性化不仅是允许的，而且是鼓励的。

> 最终的目标是让人们能够创建自己的空间、自己的社区，以自己的想法修改软件，而不牺牲来自不同社区的人们相互交流的能力。
>
> -- Eugen Rochko, Feb 20 2017, ["The power to build communities: A response to Mark Zuckerberg"](https://blog.joinmastodon.org/2017/02/the-power-to-build-communities/)

> 去中心化是数字世界的生物多样性，是健康生态系统的标志。像fediversity这样的分散式网络允许不同的用户界面、不同的软件、不同形式的政府共存与合作。
>
> -- Eugen Rochko, Dec 30 2018, ["Why does decentralization matter?"](https://blog.joinmastodon.org/2018/12/why-does-decentralization-matter/)

## 选择你的旅程 {#next-steps}

学习如何使用长毛象：

{{< page-ref page="user/signup.md" >}}

学习如何安装长毛象：

{{< page-ref page="admin/prerequisites.md" >}}

学习如何为长毛象编写应用程序：

{{< page-ref page="client/intro.md" >}}

了解长毛象后端和如何作出贡献：

{{< page-ref page="dev/overview.md" >}}




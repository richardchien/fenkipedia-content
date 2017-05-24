---
title: 如何使用 CCZU 小开机器人
created: 2016-12-30 20:08:00
author: Richard Chien
---

CCZU 小开机器人是常州大学开发者协会开发的一个同时支持 QQ 和微信的机器人（QQ 号：1647869577，微信号：cczu_xiaokai），可以对消息进行自动处理，并完成所要求的操作。

对于普通用户，小开机器人提供一些基本的常用功能，并且比较易于使用，对于高级用户，提供更多自由度比较高的强大功能。

## 使用方法

首先你需要了解「命令」的概念，「命令」由「命令名」和「参数」两部分构成。「命令名」为小开内置的功能的名称，通常一个功能有多个名称（命令名）与之对应，从而能够尽量避免由于记错命令名而造成困惑；「参数」是在使用命令时你需要告诉小开的东西（有时候可能没有），比如查天气时你需要告诉小开要你查的城市。

下面给出几个命令的例子：

- 查天气 常州
- weather 南京
- 翻译到 日语 你好
- 历史上的今天
- zhihu 20160910
- note.take 昨天买了个手机
- echo woooow
- 聊天 你好啊
- 订阅 20:00 历史上的今天

注意到例子中命令名和参数之间用空格隔开了，你也可以使用冒号或逗号隔开，如：

- 翻译，こんにちは
- 查百科：常州大学

然后你需要了解「调用命令」的概念。当你需要让小开做某个操作的时候，你需要「调用命令」，也即，在「命令」（命令名+参数）的前面加上「／」或「/」或「来，」（引号中的内容），然后发送给小开，她就会按照你的指示来做相应的事情。例如：

- ／跟我念：你好
- ／翻译到 西班牙语 你是谁
- /translate 你来自哪里
- /note.clear
- 来，记笔记：我是爱你的，看见就爱上了，就像一个人手里一只鸽子飞走了。

下图是调用「历史上的今天」命令的例子：

![](https://ww4.sinaimg.cn/large/006tNbRwgw1fb93x5lvhlj30ku112wjs.jpg)

后面将给出对于不同用户的使用建议和详细的命令列表。

## 如果你是普通用户

目前所支持的所有功能和其所对应的命令名、所需参数描述，如下表：

| 功能               | 所需参数（下面描述用分号分隔多个参数，调用时用空格隔开）             | 命令名（一行一个，第一个为主命令名）             |
| ---------------- | ---------------------------------------- | ------------------------------ |
| 获取使用帮助           | -                                        | core.help                      |
| ↑                | ↑                                        | help                           |
| ↑                | ↑                                        | 帮助                             |
| ↑                | ↑                                        | 用法                             |
| ↑                | ↑                                        | 使用帮助                           |
| ↑                | ↑                                        | 使用指南                           |
| ↑                | ↑                                        | 使用说明                           |
| ↑                | ↑                                        | 使用方法                           |
| ↑                | ↑                                        | 怎么用                            |
| 让机器人重复一段内容       | 要重复的内容                                   | core.echo                      |
| ↑                | ↑                                        | echo                           |
| ↑                | ↑                                        | 重复                             |
| ↑                | ↑                                        | 跟我念                            |
| 跟图灵机器人聊天         | 要发送给图灵机器人的内容                             | ai.tuling123                   |
| ↑                | ↑                                        | tuling123                      |
| ↑                | ↑                                        | chat                           |
| ↑                | ↑                                        | 聊天                             |
| 跟微软小冰聊天          | 要发送给小冰的内容                                | ai.xiaoice                     |
| ↑                | ↑                                        | xiaoice                        |
| ↑                | ↑                                        | 小冰                             |
| 记录一条笔记           | 要记入笔记的内容                                 | note.take                      |
| ↑                | ↑                                        | note.add                       |
| ↑                | ↑                                        | 记笔记                            |
| ↑                | ↑                                        | 添加笔记                           |
| 列出所有笔记           | -                                        | note.list                      |
| ↑                | ↑                                        | 列出所有笔记                         |
| ↑                | ↑                                        | 查看所有笔记                         |
| ↑                | ↑                                        | 所有笔记                           |
| 删除一条笔记           | 要删除的笔记 ID                                | note.remove                    |
| ↑                | ↑                                        | note.delete                    |
| ↑                | ↑                                        | 删除笔记                           |
| 清空所有笔记           | -                                        | note.clear                     |
| ↑                | ↑                                        | 清空笔记                           |
| ↑                | ↑                                        | 清空所有笔记                         |
| ↑                | ↑                                        | 删除所有笔记                         |
| 获取知乎日报           | （可选）要获取的日期，格式：20161230，默认获取当天            | zhihu.zhihu_daily              |
| ↑                | ↑                                        | zhihu-daily                    |
| ↑                | ↑                                        | zhihu                          |
| ↑                | ↑                                        | 知乎日报                           |
| 订阅知乎日报           | （可选）`-f` 标记是否覆盖以前的订阅，默认提示选择；（可选）要订阅的时间，格式：20:30，默认提示输入 | zhihu.subscribe                |
| ↑                | ↑                                        | 订阅知乎日报                         |
| 取消订阅知乎日报         | -                                        | zhihu.unsubscribe              |
| ↑                | ↑                                        | 取消订阅知乎日报                       |
| 查询天气             | 要查询的城市                                   | weather.weather                |
| ↑                | ↑                                        | weather                        |
| ↑                | ↑                                        | 天气                             |
| ↑                | ↑                                        | 查天气                            |
| ↑                | ↑                                        | 天气预报                           |
| ↑                | ↑                                        | 查天气预报                          |
| 查询生活指数（由天气派生）    | 要查询的城市                                   | weather.suggestion             |
| ↑                | ↑                                        | suggestion                     |
| ↑                | ↑                                        | 生活指数                           |
| ↑                | ↑                                        | 生活建议                           |
| ↑                | ↑                                        | 天气建议                           |
| 订阅一条命令           | （可选）需要推送的时间；（可选）要订阅的命令（命令名+参数）           | subscribe.subscribe            |
| ↑                | ↑                                        | subscribe                      |
| ↑                | ↑                                        | 订阅                             |
| 查看已经订阅的所有命令      | -                                        | subscribe.subscribe_list       |
| ↑                | ↑                                        | subscribe_list                 |
| ↑                | ↑                                        | subscribe-list                 |
| ↑                | ↑                                        | 订阅列表                           |
| ↑                | ↑                                        | 查看订阅                           |
| ↑                | ↑                                        | 查看所有订阅                         |
| ↑                | ↑                                        | 所有订阅                           |
| 取消订阅一条命令         | 要取消订阅的 ID（可通过「查看所有订阅」看到）                 | subscribe.unsubscribe          |
| ↑                | ↑                                        | unsubscribe                    |
| ↑                | ↑                                        | 取消订阅                           |
| 获取数字人民币金额的汉字大写形式 | 要大写的数字金额                                 | simpletools.money_zh           |
| ↑                | ↑                                        | money_zh                       |
| ↑                | ↑                                        | money-zh                       |
| ↑                | ↑                                        | 人民币大写                          |
| ↑                | ↑                                        | 金额大写                           |
| ↑                | ↑                                        | 人民币金额大写                        |
| 生成短链接            | 要生成短链接的原链接                               | simpletools.short_url          |
| ↑                | ↑                                        | short_url                      |
| ↑                | ↑                                        | short-url                      |
| ↑                | ↑                                        | 生成短网址                          |
| ↑                | ↑                                        | 生成短链接                          |
| ↑                | ↑                                        | 短网址                            |
| ↑                | ↑                                        | 短链接                            |
| 查询百科             | 要查询的关键词                                  | simpletools.baike              |
| ↑                | ↑                                        | baike                          |
| ↑                | ↑                                        | 百科                             |
| ↑                | ↑                                        | 查百科                            |
| 获取一个笑话           | -                                        | simpletools.joke               |
| ↑                | ↑                                        | joke                           |
| ↑                | ↑                                        | 笑话                             |
| ↑                | ↑                                        | 说笑话                            |
| ↑                | ↑                                        | 说个笑话                           |
| 获取历史上的今天         | -                                        | simpletools.today\_in\_history |
| ↑                | ↑                                        | today\_in\_history             |
| ↑                | ↑                                        | today-in-history               |
| ↑                | ↑                                        | 历史上的今天                         |
| 翻译一段文本（到命令名的语言）  | 要翻译的文本                                   | translate.translate            |
| ↑                | ↑                                        | translate                      |
| ↑                | ↑                                        | 翻译                             |
| ↑                | ↑                                        | 翻訳                             |
| 翻译一段文本到指定的目标语言   | 目标语言；要翻译的文本                              | translate.translate_to         |
| ↑                | ↑                                        | translate_to                   |
| ↑                | ↑                                        | translate-to                   |
| ↑                | ↑                                        | 翻译到                            |
| ↑                | ↑                                        | 翻译成                            |
| 查询域名或 IP 的所在地    | 要查询的域名或 IP                               | networktools.ip                |
| ↑                | ↑                                        | ip                             |
| 获取字符串的 Base64 编码 | 要编码的内容                                   | encode.base64                  |
| ↑                | ↑                                        | base64                         |
| 解码 Base64 字符串    | 要解码的内容                                   | encode.base64_decode           |
| ↑                | ↑                                        | base64_decode                  |
| ↑                | ↑                                        | base64-decode                  |
| ↑                | ↑                                        | base64d                        |
| 获取字符串的 MD5 编码    | 要编码的内容                                   | encode.md5                     |
| ↑                | ↑                                        | md5                            |
| 获取字符串的 SHA1 编码   | 要编码的内容                                   | encode.sha1                    |
| ↑                | ↑                                        | sha1                           |
| 获取字符串的 SHA256 编码 | 要编码的内容                                   | encode.sha256                  |
| ↑                | ↑                                        | sha256                         |
| 获取随机数            | （可选）最小范围（整型，默认为 1，包含）；（可选）最大范围（整型，包含）；（可选）要获取的个数，格式 `x12`、`x100` 这样，默认 1 个 | random.number                  |
| ↑                | ↑                                        | 随机数                            |
| 获取随机字符           | （可选）字符选择范围（作为连续的一个字符串参数传入，默认为拉丁字母和阿拉伯数字）；（可选）要获取的个数，格式 `x12`、`x100` 这样，默认 1 个 | random.char                    |
| ↑                | ↑                                        | 随机字符                           |
| 随机化序列            | 需要随机化的序列，每个元素用逗号或空格隔开                    | random.shuffle                 |
| ↑                | ↑                                        | 随机化                            |
| 查询 B 站新番         | （可选）要查询的年份和开播月份，格式如「17-01」，默认查当前季度       | bilibili.anime_index           |
| ↑                | ↑                                        | anime_index                    |
| ↑                | ↑                                        | anime-index                    |
| ↑                | ↑                                        | 番剧索引                           |
| ↑                | ↑                                        | 番剧                             |
| ↑                | ↑                                        | 新番                             |
| 查询 B 站新番更新时间表    | （可选）要查询的日期，格式如「2-23」或「2」，前一种格式表示月和日，后一种格式表示和今天相差的天数，「0」为今天、「1」为明天；（可选）要查询的动漫名称（两个可选至少填一个） | bilibili.anime_timeline        |
| ↑                | ↑                                        | anime_timeline                 |
| ↑                | ↑                                        | anime-timeline                 |
| ↑                | ↑                                        | 番剧时间表                          |
| ↑                | ↑                                        | 新番时间表                          |

## 如果你是高级用户

除了上面的普通命令，小开机器人还提供了一个 scheduler 系列命令，用于自定义计划任务，如定时触发若干设置好的命令，类似于 Linux 上的 Cron。列表如下：

| 功能                        | 所需参数        | 命令名                   |
| ------------------------- | ----------- | --------------------- |
| 添加一个计划任务                  | 见注释 1       | scheduler.add_job     |
| ↑                         | ↑           | scheduler.add-job     |
| ↑                         | ↑           | scheduler.add         |
| 删除一个计划任务                  | 要删除的计划任务 ID | scheduler.remove_job  |
| ↑                         | ↑           | scheduler.remove-job  |
| ↑                         | ↑           | scheduler.remove      |
| 查询一个计划任务                  | 要查询的计划任务 ID | scheduler.get_job     |
| ↑                         | ↑           | scheduler.get-job     |
| ↑                         | ↑           | scheduler.get         |
| 列出所有计划任务                  | -           | scheduler.list_jobs   |
| ↑                         | ↑           | scheduler.list-jobs   |
| ↑                         | ↑           | scheduler.list        |
| 手动执行一个计划任务                | 要执行的计划任务 ID | scheduler.execute_job |
| ↑                         | ↑           | scheduler.execute-job |
| ↑                         | ↑           | scheduler.execute     |
| ↑                         | ↑           | scheduler.exec        |
| ↑                         | ↑           | scheduler.trigger     |
| ↑                         | ↑           | scheduler.do          |
| 计算 Cron 时间表达式接下来 7 次的触发时间 | Cron 时间表达式  | scheduler.cron_check  |
| ↑                         | ↑           | cron_check            |
| ↑                         | ↑           | cron-check            |
| ↑                         | ↑           | cron_test             |
| ↑                         | ↑           | cron-test             |

注释 1：由于参数比较复杂，请先调用 `scheduler.add_job --help` 查看帮助信息。

## 如果你是程序员

小开机器人的后台程序是使用 Python 编写的，源码在 [CCZU-DEV/xiaokai-bot](https://github.com/CCZU-DEV/xiaokai-bot)。

如果有需要，你可以自行编写插件（见 [XiaoKai Bot 文档](https://cczu-dev.github.io/xiaokai-bot/)），编写后你可以发送 Pull Request 申请合并到原项目，或者也可以你自己部署机器人。

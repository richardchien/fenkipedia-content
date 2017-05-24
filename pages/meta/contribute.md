---
title: Fenkipedia:帮助完善词条
created: 2016-08-17 12:40:00
---

我们迫切需要热心的志愿者来帮助我们完善词条，如果你对某些本站还没有的词条有所了解和研究，欢迎你的加入。

你可以通过 GitHub 直接贡献词条，或者通过邮箱 admin@fenkipedia.cn 与我们联系。

## 通过 GitHub 贡献

首先你需要有一个 GitHub 账号，如果还没有，可以在 [这里](https://github.com) 注册。

登录 GitHub 之后，前往 https://github.com/richardchien/fenkipedia-content 并点击「Fork」，从而复制一份到你自己的代码仓库，然后在你自己的那一份拷贝中，进入你想要添加词条的目录，点击「Create new file」，此时会跳转到编辑页面，将文件命名为 `词条名.md` 的形式，然后使用 Markdown 语法编写词条内容，注意：你需要在文件的第一行填写形如 `created: 2016-08-17 00:13:00` 的创建日期，如果是修改文件，则再添加一个 `updated: 2016-08-17 00:13:00` 表示更新时间，如果你还需要网站在展示词条内容时采用和文件名中的词条名不同的文字作为标题，请在文件开头添加一行形如 `title: 词条展示页面的标题` 的内容，这三个开头的标记内容的前后使用 `---` 隔开，例如：

```md
---
title: 首页
date: 2016-08-16 19:52:00
updated: 2016-08-17 12:50:00
---

欢迎来到 Fenkipedia 冯基百科！
```

如果你对 Markdown 不太了解，可以查看 [这里](http://wowubuntu.com/markdown/) 或参考其它已经存在的词条，当然你也可以使用邮件的方式贡献你的词条，我们会帮你把词条发布出来。

词条内容编写完成后点击页面底部的「Commit new file」提交，成功之后，新添加的词条将出现在你 Fork 的这个仓库中，你还需要点击仓库首页的「New pull request」，然后「base fork」选择「richardchien/fenkipedia-content」，「head fork」选择你的 Fork，如果显示「Able to merge」就可以点击「Create pull request」来创建 Pull Request，填写 Pull Request 的标题和内容，你需要在这里注明你添加或修改词条的原因或其它说明，再次点击「Create pull request」之后便创建成功，我们会及时将你的词条合并进入网站。

## 通过邮件贡献

如果你不方便使用 GitHub 来贡献你的词条，也可以通过联系我们的邮箱 admin@fenkipedia.cn 来提供内容，请在邮件标题注明「贡献词条 XXX」，并附上词条内容，我们会尽快将你贡献的词条发布到网站。

## 致谢

每一个为我们贡献词条的热心志愿者都将会被记录在 [志愿者](/meta/volunteers) 页面作为感谢，如果你有其它需求，比如指定该页面上显示的你的名字等，请在 Pull Request 或邮件中说明。

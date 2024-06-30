---
title: 欢迎来到912秘密花园
---

This is a blank Quartz installation.
See the [documentation](https://quartz.jzhao.xyz) for how to get started.

---

以上为空白存档介绍，这里是一些912专业课备考素材。

# 目录
[[数据结构]]

[[组成原理]]


---
# 如何使用quartz发布Obsidian笔记（个人记录）
主要参考：[如何使用 Quartz 4.0 和 GitHub Pages 免费发布 Obsidian 笔记 (insile.github.io)](https://insile.github.io/my-notes/%E7%AC%94%E8%AE%B0/%E5%85%AC%E5%85%B1%E7%AC%94%E8%AE%B0%E5%BA%93/%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8-Quartz-4.0-%E5%92%8C-GitHub-Pages-%E5%85%8D%E8%B4%B9%E5%8F%91%E5%B8%83-Obsidian-%E7%AC%94%E8%AE%B0)

官方文档：[Welcome to Quartz 4 (jzhao.xyz)](https://quartz.jzhao.xyz/)

其他参考：
- [使用Quartz 发布 Obsidian (lgf4591.github.io)](https://lgf4591.github.io/quartz-obsidian/Pages/%E4%BD%BF%E7%94%A8Quartz-%E5%8F%91%E5%B8%83-Obsidian)
- [使用Quartz部署Obsidian笔记网站 | Wong's Blog (wssh.trade)](https://blog.wssh.trade/posts/obsidian-quartz/)


注意事项：
1. 步骤1中，默认选择Empty Quartz --> Treat links as shortest path，即在content文件夹中创建一个空白库，后续再添加笔记。若已有撰写好的Obsidian库，可以选择Copy（复制）或者Symlink（快捷方式链接），但本人均未尝试过。
2. 在我配置完成后，每次同步需要先进行`npm quartz sync`然后再进行`git push`才能更新，不知道是哪里出了问题，期待解决。
3. 每次进行`npm quartz sync`后均会出现`Error: EBUSY: resource busy or locked, rmdir 'D:\Quartz\quartz\content'`字样的报错，但不影响同步以及网页发布，期待解决。
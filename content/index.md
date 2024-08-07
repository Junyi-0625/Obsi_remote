---
title: 欢迎来到912秘密花园
---

This is a blank Quartz installation.
See the [documentation](https://quartz.jzhao.xyz) for how to get started.

---

以上为空白介绍页存档，这里是一些912专业课备考素材。

# 目录
[[数据结构]]

[[组成原理]]


---
# 如何使用Quartz发布Obsidian笔记（个人记录）
主要参考：[如何使用 Quartz 4.0 和 GitHub Pages 免费发布 Obsidian 笔记 (insile.github.io)](https://insile.github.io/my-notes/%E7%AC%94%E8%AE%B0/%E5%85%AC%E5%85%B1%E7%AC%94%E8%AE%B0%E5%BA%93/%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8-Quartz-4.0-%E5%92%8C-GitHub-Pages-%E5%85%8D%E8%B4%B9%E5%8F%91%E5%B8%83-Obsidian-%E7%AC%94%E8%AE%B0)

官方文档：[Welcome to Quartz 4 (jzhao.xyz)](https://quartz.jzhao.xyz/)

其他参考：
- [使用Quartz 发布 Obsidian (lgf4591.github.io)](https://lgf4591.github.io/quartz-obsidian/Pages/%E4%BD%BF%E7%94%A8Quartz-%E5%8F%91%E5%B8%83-Obsidian)
- [使用Quartz部署Obsidian笔记网站 | Wong's Blog (wssh.trade)](https://blog.wssh.trade/posts/obsidian-quartz/)


注意事项：
1. 在主要参考网页的步骤1中，默认选择Empty Quartz --> Treat links as shortest path，即在content文件夹中创建一个空白库，后续再添加笔记。若已有撰写好的Obsidian库，可以选择Copy（复制）或者Symlink（快捷方式链接），但我都没有尝试过，选择后可能需要修改路径选项。
2. 每次同步前需要**关闭**Obsidian中打开的content库，再在终端（或Powershell/命令行）中输入`npx quartz sync`，否则会**可能**出现3中的问题（大概类似word文档没关闭的时候不能直接复制...？但有时候会自动关闭）。
3. 每次同步时，终端中的`npx quartz sync`执行完成后均会出现`Error: EBUSY: resource busy or locked, rmdir 'D:\Quartz\quartz\content'`字样的报错，查看github仓库发现并未更新，此时输入`git push`命令才能完成同步。
4. Quartz网页中的格式、字样与Obsidian中的略有区别，最重要的一点是Obsidian中两次换行相当于网页中的一次换行（类似Latex），其他格式要求参考官方文档。
5. 出现`fatal: unable to access 'https://github.com/Junyi-0625/Obsi_remote/': HTTP/2 stream 1 was not closed cleanly before end of the underlying stream`报错，参考[【Git】unable to access https://github.com/xxx/xxx: HTTP/2 stream 1 was not closed cleanly before-CSDN博客](https://blog.csdn.net/m0_47406832/article/details/123044722)进行解决。
---
title: 使用hexo发文报错can not read a block mapping entry
date: 2022-02-12 23:31:58
tags:
---

今天使用hexo发文时候，输入`hexo g`的时候报错：

`can not read a block mapping entry; a multiline key may not be an implicit key at line *, column *:`

上网转了一圈发现是设置tag属性之后没有加空格，导致报错，甚至整个博客页面崩溃。

所以要严格按照语法来写文章头部。

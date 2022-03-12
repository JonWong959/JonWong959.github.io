---
title: hexo博客推送github显示鉴权失败
date: 2022-02-12 23:21:04
tags: 问题解决
---

更换新电脑，部署hexo博客的时候，向仓库推时报错，显示鉴权失败，记录下解决办法。



## 解决过程

#### 环境说明

客户端：macOS M1芯片

托管平台：github

#### 问题描述：

在使用`hexo d`推送时，出现鉴权失败错误。

## 解决方案

修改站点配置文件`_config.yml`

```
# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
deploy:
  type: git
  repo: git@github.com:JonWong959/JonWong959.github.io.git
  branch: master
```

把repo从https地址改成SSH地址。

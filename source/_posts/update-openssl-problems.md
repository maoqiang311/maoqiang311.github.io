---
title: openssl版本升级
date: 2024-03-27 17:26:11
tags:
---
主要记录openssl从1.0.2t版本升级到1.1.1w版本遇到的一些问题和解决方案

### openssl源码中新增接口

先在源码中加入接口，然后`./config`生成`makefile`文件
`make update`将新加接口加载到文件中，然后再`make && make install`即可
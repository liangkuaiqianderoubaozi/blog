---
title: springboot
author: roubaozi
date: 2022-04-24
category: Jekyll
layout: post
---

2.6.7版本pgeHelper循环依赖问题-com.github.pagehelper.autoconfigure.PageHelperAutoConfiguration
-------------
新项目使用pageHelper的时候，项目启动后出现的情况
![0423.png](https://liangkuaiqianderoubaozi.github.io/blog/gitbook/resources/springboot/0423.png)

springboot2.6.x禁止循环依赖，springboot降级到2.3.3版本，或者升级 pageHelper>=1.4.1.
~~~
   <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
<!--        <version>2.6.7</version>-->
        <version>2.3.3.RELEASE</version>
    </parent>
~~~








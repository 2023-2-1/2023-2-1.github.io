---
title: Welcome
tags: TeXt
---

# SpringBoot自动装配原理

在启动类中的 run 方法中传入启动类（方便后续获取其注解信息）
执行 run 方法，创建 SpringApplication 对象，并调用 LoadSpringFactories() 方法，将/META-INF/spring.factories文件里的 k-v 读入缓存 （方便后面使用）
继续执行 run 方法，获取传入的启动类，并解析上面的注解，当解析到 @Import（{AutoConfigurationImportSelector.class}）时，会将 AutoConfigurationImportSelector 加载进方法区，通过反射创建对象，调用






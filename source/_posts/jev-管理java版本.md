---
title: jev 管理java版本
date: 2016-01-16 14:00:56
tags: 
- java
- tool
---

Use jenv is an easy way.

1.Install jenv

    curl -s get.jenv.io | bash
2.Config jenv

    cd ~/.jenv/candidates/
    mkdir java
    cd java
    mkdir 1.7
    mkdir 1.8
3.Symlink the jdk path

    ln -s /Library/Java/JavaVirtualMachines/jdk1.7.0_79.jdk/Contents/Home/bin ~/.jenv/candidates/java/1.7
    ln -s /Library/Java/JavaVirtualMachines/jdk1.8.0_45.jdk/Contents/Home/bin ~/.jenv/candidates/java/1.8
4.You are all set

switch command:

jenv use java 1.8
set default:

jenv default java 1.7
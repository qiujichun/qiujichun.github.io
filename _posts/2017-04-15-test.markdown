---
layout: post
title:  "Welcome to TonyChiu!"
date:   2017-04-11 15:41:08 +0800
categories: tonychiu update
---

# Author: Tony Chiu
# Blog: http://www.chiushi.com
# Github: https://github.com/qiujichun
# Email: qiujichun@gmail.com
# Official Accounts: 

1、定义两大主功能

    注册 登录

2、默认注册用户类型为“普通用户”

3、登录

    a、登录的账户为“普通账户”，具有的权限为：
        ·查看本账户信息
        ·修改本账户密码

    b、登录的账户为“管理员账户”，具有的权限为：
        ·查看本账户信息
        ·修改本账户密码
        ·添加用户（普通）
        ·删除用户
        ·搜索用户（支持精确和模糊）
        ·提高权限
        ·查看所有用户
        ·修改普通用户密码

4、系统界面

    a、注册
        --- Welcome To The User Management Program ---
                 1.注册           2.登录
        ----------------------*-----------------------
        请键入您要的操作：1
        请输入新的用户名:test
        请输入密码:test
        请输入邮箱:test@demo.com
        恭喜！注册成功
    
    b、登录（普通用户）
        请键入您要的操作：2
        请输入用户名:user1
        请输入密码:user1
        欢迎user1登录
        ------ 您可以进行的操作 ------
        1.查看信息；2.修改密码；q.退出
        
        键入您的选择：1
        ***用户信息如下***
        用户名：user1，邮箱：user1@demo.com，账户类型：普通用户
        
    c、登录（管理员）
        请键入您要的操作：2
        请输入用户名:admin
        请输入密码:admin
        欢迎admin登录
        ------------------------------------------------ 您可以进行的操作 ------------------------------------------------
        1.查看信息；2.修改密码；3.添加用户；4.删除用户；5.搜索用户；6.提高权限；7.查看所有用户；8.修改普通用户密码；q.退出
        
        键入您的选择：7
        ***用户信息如下***
        用户名：admin，邮箱：admin@demo.com，账户类型：管理员
        用户名：user1，邮箱：user1@demo.com，账户类型：普通用户
        用户名：user2，邮箱：user2@demo.com，账户类型：普通用户
        用户名：user3，邮箱：user3@demo.com，账户类型：普通用户
        用户名：test，邮箱：test@demo.com，账户类型：普通用户
        
        键入您的选择：5
        请输入要搜索的用户信息:user1
        用户名：user1，邮箱：user1@demo.com，账户类型：普通用户
        
        键入您的选择：5
        请输入要搜索的用户信息:@demo.com
        用户名：admin，邮箱：admin@demo.com，账户类型：管理员
        用户名：user1，邮箱：user1@demo.com，账户类型：普通用户
        用户名：user2，邮箱：user2@demo.com，账户类型：普通用户
        用户名：user3，邮箱：user3@demo.com，账户类型：普通用户
        用户名：test，邮箱：test@demo.com，账户类型：普通用户

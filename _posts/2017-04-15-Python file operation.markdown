---
layout: post
title:  "Python 文件操作-总结"
date:   2017-04-15 15:57:08 +0800
categories: python file
---

# Author: Tony Chiu
# Blog: http://www.chiushi.com
# Github: https://github.com/qiujichun
# Email: qiujichun@gmail.com
# Official Accounts: ![](http://i.imgur.com/d4Uh1kD.jpg)

**一、打开文件**

文件句柄 = open('文件路径', '模式')
打开文件时，需要指定文件路径和以何等方式打开文件，打开后，即可获取该文件句柄，日后通过此文件句柄对该文件操作。
打开文件的模式有：

	* r ，只读模式【默认】
	* w，只写模式【不可读；不存在则创建；存在则清空内容；】
	* x， 只写模式【不可读；不存在则创建，存在则报错】
	* a， 追加模式【可读；   不存在则创建；存在则只追加内容；】

"+" 表示可以同时读写某个文件

	* r+， 读写【可读，可写】
	* w+，写读【可读，可写】
	* x+ ，写读【可读，可写】
	* a+， 写读【可读，可写】

 "b"表示以字节的方式操作

	* rb  或 r+b
	* wb 或 w+b
	* xb 或 w+b
	* ab 或 a+b


 注：以b方式打开时，读取到的内容是字节类型，写入时也需要提供字节类型

**二、文件指针（位置）**

	* 默认在首位
	* 执行读read()无参数操作后，读全部到尾部
	* tell读取当前指针位置（永远以字节方式）
	* seek调整指针位置（永远以字节方式）
	* 英文字母占一个字节，而中文是三个字节，由于seek永远是以字节方式；所以当seek位置正好处于中文字节位置中时，会乱码


**三、文件操作**

	* flush()强制刷新（写到硬盘）
	* truncate截断（把指针后面的内容清空）


**四、文件关闭**

f.open('file1','r')
f.close()

with open('file1','r') as f1:
with open('file1','r') as f1, open('file2','r') as f2 :   # 同时打开多个（python2.6不支持）

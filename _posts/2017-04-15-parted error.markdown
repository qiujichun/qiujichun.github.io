---
layout: post
title:  "parted 分区报错"
date:   2017-04-15 16:41:08 +0800
categories: linux 
---

# Author: Tony Chiu
# Blog: http://www.chiushi.com
# Github: https://github.com/qiujichun
# Email: qiujichun@gmail.com
# Official Accounts: ![](http://i.imgur.com/ZwXXRpR.jpg)


**1、报错**

Error: partition length of 6442450944 sectors exceeds the loop-partition-table-imposed maximum of 4294967295

**2、原因**

This error means that you can't create a partition of more than 2 TiB on an MBR-partitioned disk. You must use GPT partitioning

**3、解决**

parted /dev/_vdb_ mklabel gpt

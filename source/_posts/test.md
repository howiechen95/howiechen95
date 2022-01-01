---
title: Themes Test
date: 2021-06-23 01:04:34
updated:
tags: 
    - 测试  
categories: 
    - 测试
top_img: https://howiechen95.com/group1/M00/00/00/CgAMB2DSxaWAO-nPAAfmKyslh6072.jpeg
cover: https://howiechen95.com/group1/M00/00/00/CgAMB2DSxbGAPK8fAAYFfV3kaq801.jpeg  
comments: comments
toc:   
toc_number:  
copyright:  
copyright_author: Howie  
copyright_author_href:   
copyright_url:  
copyright_info:  
mathjax:  
katex:  
aplayer:  
highlight_shrink:  
aside:
---

# [Butterfly 安裝文檔(三) 主題配置-1 | Butterfly](https://butterfly.js.org/posts/4aa8abbe/)

### 记录测试情况

> 使用自己搭建的文件系统，在 github page 引用图片存在跨域问题，在手机上却没发现
> 后来在自己搭建文件服务器上的允许hexo，就不再跨域了
> 可能周末还是得把域名备案的事搞一下


```sql
CREATE TABLE IF NOT EXISTS `runoob_tbl`(
   `runoob_id` INT UNSIGNED AUTO_INCREMENT,
   `runoob_title` VARCHAR(100) NOT NULL,
   `runoob_author` VARCHAR(40) NOT NULL,
   `submission_date` DATE,
   PRIMARY KEY ( `runoob_id` )
)ENGINE=InnoDB DEFAULT CHARSET=utf8;
```

```golang
package bot

import (
	"fmt"
	"time"
)

// Je pense, donc je suis
type Bot struct {
	Skills map[int64]Skill
	Souls  map[int64]Soul
	Status map[int64]Status
	DNA    map[int64]DNA
	Feel   map[int64]Feel
	Skill  map[int64]Skill
}

func New() (bot *Bot) {
	bot = &Bot{
		Skills: make(map[int64]Skill),
		Souls:  make(map[int64]Soul),
		Status: make(map[int64]Status),
		DNA:    make(map[int64]DNA),
		Feel:   make(map[int64]Feel),
		Skill:  make(map[int64]Skill),
	}
	return
}

func (b *Bot) Awake() {
	for ; b.Status[CoreStatus].statusType != DeadStatus; {
		fmt.Println(time.Now().Unix(), " i am alive")
		time.Sleep(1 * time.Second)
	}
}

func (b *Bot) reload() {
	b.loadFromFile()
}

func (b *Bot) loadFromFile() {

}

type Soul struct {
}

// by create
type DNA struct {
}

// outside & inside
type Feel struct {
}

func (f *Feel) ou() {

}

// imitate
type Skill struct {
	skillType int64
}

const (
	CoreStatus = 0
)
const (
	DeadStatus = int64(-1)
)

type Status struct {
	statusType int64
}

```

{% gallery %}
![](https://i.loli.net/2019/12/25/Fze9jchtnyJXMHN.jpg)
![](https://i.loli.net/2019/12/25/ryLVePaqkYm4TEK.jpg)
![](https://i.loli.net/2019/12/25/gEy5Zc1Ai6VuO4N.jpg)
![](https://i.loli.net/2019/12/25/d6QHbytlSYO4FBG.jpg)
![](https://i.loli.net/2019/12/25/6nepIJ1xTgufatZ.jpg)
![](https://i.loli.net/2019/12/25/E7Jvr4eIPwUNmzq.jpg)
![](https://i.loli.net/2019/12/25/mh19anwBSWIkGlH.jpg)
![](https://i.loli.net/2019/12/25/2tu9JC8ewpBFagv.jpg)
{% endgallery %}

{% note simple %}
默認 提示塊標籤
{% endnote %}

{% note default simple %}
default 提示塊標籤
{% endnote %}

{% note primary simple %}
primary 提示塊標籤
{% endnote %}

{% note success simple %}
success 提示塊標籤
{% endnote %}

{% note info simple %}
info 提示塊標籤
{% endnote %}

{% note warning simple %}
warning 提示塊標籤
{% endnote %}

{% note danger simple %}
danger 提示塊標籤
{% endnote %}


## 看板娘配置

```
npm install --save hexo-helper-live2d
```
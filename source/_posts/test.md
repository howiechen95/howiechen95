---
title: Themes Test
date: 2021-06-23 01:04:34
updated:
tags: 测试  
categories: 测试
top_img: 'linear-gradient(20deg, #0062be, #925696, #cc426e, #fb0347)'
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

```

{% gallery %}
{% endgallery %}

```
---
layout: post
title: "gorm update"
description: "gorm update"
keywords: "gorm update"
category: "go gorm"
tags: [go,gorm,update]
---

## 参考资料


## 1. 细节
Where语句要写在Update之前，否则Where条件带不上；
query := db.Model(&table).Where("field1=?", value1).Update("locked",true})
if err := query.Error; err != nil {
	logger.Error(err)
	return
}
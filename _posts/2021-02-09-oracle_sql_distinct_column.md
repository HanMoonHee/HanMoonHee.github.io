---
layout: post
title:  "[sql] 데이터 중복과 null값을 제외하여 count하기"
date:   2021-02-09 00:00:00 +0700
categories: [sql]
---

```sql
SELECT count(distinct column) from table;
```

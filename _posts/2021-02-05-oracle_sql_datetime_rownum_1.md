---
layout: post
title:  "[sql] 가장 빠른 날짜의 데이터를 조회하는 방법"
date:   2021-02-09 12:50:00 +0700
categories: [sql]
---

```sql
SELECT column from (
    select column from table order by datetime
) where rownum = 1;
```

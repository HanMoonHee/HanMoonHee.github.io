---
layout: post
title:  "[sql] GROUP BY를 활용하여 데이터 그룹화"
date:   2021-02-09 00:00:00 +0700
categories: [sql]
---

COLUMN1의 중복된 데이터를 그룹화하여 COLUMN1을 기준으로 COLUMN2를 COUNT하는 쿼리문

```sql
SELECT COLUMN1, count(COLUMN2) from TABLE group by COLUMN1;
```

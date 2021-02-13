---
layout: post
title:  "[sql] GROUP화된 필드를 HAVING절을 이용하여 조건주기"
date:   2021-02-13 00:00:00 +0700
categories: [sql]
---

HAVING절은 GROUP BY 된 필드를 기준으로 조건을 줄 수 있다.

```sql
SELECT   name,
         count(name) as count
from     animal_ins
group by name
having   count(name) > 1
order by name asc;
```

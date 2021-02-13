---
layout: post
title:  "[sql] 서브쿼리, TO_CHAR함수를 활용하여 시간대별 데이터를 추출하기"
date:   2021-02-13 00:00:00 +0700
categories: [sql]
---

09:00부터 19:59까지, 각 시간대별로 입양이 몇 건이나 발생했는지 조회하는 SQL문을 작성해주세요

```sql
SELECT  HOUR,
        COUNT(*)
        FROM (
            SELECT TO_CHAR(DATETIME, 'HH24') AS HOUR FROM TABLE
        )
WHERE HOUR BETWEEN 09 AND 19
GROUP BY HOUR
ORDER BY HOUR;
```

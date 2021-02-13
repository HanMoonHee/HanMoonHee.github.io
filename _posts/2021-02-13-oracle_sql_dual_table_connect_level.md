---
layout: post
title:  "[sql] 오라클 자체에서 제공되는 DUAL테이블 그리고 CONNECT BY LEVEL"
date:   2021-02-13 00:00:00 +0700
categories: [sql]
---

제목처럼 오라클 자체에서 제공되는 테이블이다.

간단하게 함수를 이용해서 계산 결과값을 확인 할 때 사용하는 테이블이다.

어느 사용자나 접근이 가능하다.


DUAL테이블을 조회하면 하나의 행을 조회가 가능한데 CONNECT BY LEVEL을 사용하면 다중 행 조회가 가능하다.

```sql
SELECT
    LEVEL
FROM DUAL
CONNECT BY LEVEL <7;
```

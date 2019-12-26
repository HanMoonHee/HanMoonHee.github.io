---
layout: post
title:  "[Oracle] 내가 보려고 만드는 많이 쓰는 오라클 쿼리문 정리 복습"
# date:   2019-05-13 18:34:10 +0700
date:   2019-10-14 00:00:00 +0700
categories: [oracle]
---

<br />

### 데이터 개수
~~~
select count(*) from tableName
~~~

### 테이블 삭제
~~~
drop table tableName
~~~

### 특정 개수만큼 테이블 목록 불러오기 
~~~
<![CDATA[
    select * from 
    (select rownum rn, tt. * from
    (select * from tableName order by seq desc)tt
    )where rn>=#{startNum} and rn<=#{endNum}
]]>

*startNum과 endNum은 프런트에서 데이터를 받아온다.
*<![CDATA[]]>를 쓰는이유는 쿼리문 작성시 부등호 등을 쓸 일이 있는데 < 와 같은 기호는 괄호인지 비교연산자 인지 확인이 지않기때문에 이외에도 특수문자 사용하는데 제한이있기떄문이다.
~~~

### 테이블에 특정 데이터 검색
~~~
select * from
(select rownum rn, tt. * from
(select * from tableName where
<foreach collection="checkbox" item="check" index="i" separator="or">
    ${checkbox[i]} like '%'||#{keyword}||'%' 
</foreach>
order by seq asc)tt
<![CDATA[
    )where rn>=#{startNum} and rn<=#{endNum}
]]>

*foreach문을 이용하여 프런트에서 여러개의 데이터를 반복적으로 검색한다
~~~

### 특정 데이터 보기
~~~
select * from tableName where seq=#{seq}

*seq값을 프런트에서 받아와 seq값에 맞는 데이터 보기
~~~

### 테이블의 특정데이터(조회수)를 증가
~~~
update tableName set hit = hit+1 where seq = #{seq}
~~~

### 테이블의 특정데이터 지우기
~~~
delete from tableName where id=#{memId} and seq=#{seq}
~~~

### 테이블 데이터 추가
~~~
insert into tableName values(SEQ_NOTICEBOARD.nextval,#{id},#{subject},#{content},0,sysdate)
~~~

### 게시판 글 열람, 수정시 정보 가져오기
~~~
select * from tableName where seq=#{seq}
~~~


----------------

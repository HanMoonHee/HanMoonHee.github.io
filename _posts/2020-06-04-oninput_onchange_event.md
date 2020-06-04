---
layout: post
title:  "[javascript]oninput, onchange란?"
date:   2020-06-04 00:00:00 +0700
categories: [javascript]
---
### 1. onsubmit

***onsubmit***은 form전송을 하기 전에 입력된 데이터의 유효성을 체크하기 위해 사용하는 이벤트 <br />
ex) onsubmit="return false"가 form에 있다면 do nothing in submit으로 전송 불가 <br />
onsubmit으로 이벤트를 걸어주면 키보드로 값을 입력할때마다 이벤트가 발생한다.

### 2. onchange
***onchange***는 SELECT BOX를 이용해 어떤 이벤트를 실행하고자 할 때는 주로 onchange 이벤트를 사용한다. <br />
input이나 select 등의 데이터가 변경될 때 호출되는 이벤트이다.

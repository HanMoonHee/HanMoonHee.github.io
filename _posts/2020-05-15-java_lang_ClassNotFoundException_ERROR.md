---
layout: post
title:  "[spring]java.lang.ClassNotFoundException에러"
date:   2020-05-14 13:00:00 +0700
categories: [spring]
---
* 내가 생성한 프로젝트가 아닌 외부에서 형상관리 등으로 가져와 나의 서버에 붙이는 과정에서 java.lang.ClassNotFoundException에러가 발생했다. 이 경우 해결법은

1. 마우스 우클릭 - properties - targeted runtimes 에서 서버 바꿔줘야됨.
2. 이클립스 프로젝트 - properties - jaba build path - order and export tab - 사용자라이브러리(jre system library)채크
3. shoppingMall의 경우 존재하지 않는 catalina 라이브러리 경로가 불러와져 에러가 나서 java build path에서 에러나는 해당 라이브러리를 지움

<img src="/static/img/posting/classNotFoundException.PNG">

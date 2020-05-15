---
layout: post
title:  "[spring]프로젝트 세팅파일 의미 정리"
date:   2020-03-15 00:00:00 +0700
categories: [spring]
---

# web.xml
1. 배포서술자(DD), 스프링 기본 환경 설정으로 서버가 처음 로딩 될 때 읽어들이고 작성된 설정을 적용하여 서버를 시작.
2. 디스패처 서블릿, 디비 커넥션, 리스너, 필터, 웹컴 파일
3. root-context.xml, security-context.xml 경로 설정
4. 서버 url pattern 설정
5. encoding(UTF-8) 설정

# servlet-context.xml
1. VIEW 지원 빈 설정
2. 컨트롤러, 인터셉터
3. CSS, JS, ASSET, IMAGE 폴더 등 을 MAPPING

# root-context.xml
1. VIEW 지원을 제외한 스프링에서 공유하는 공통 빈 설정
2. 서비스, 레파지토리

# globals.properties
1. 데이터 베이스 접속 정보
2. 단순 프로퍼티로 제한 없음

# context-datasource.xml
1. 데이터 베이스 접속 정보 파일을 서버별로 분기하여 빈 생성 및 제공

# sql-session-config.xml
1. 콘텍스트 매퍼에서 사용 할 매퍼 및 데이터 베이스 접속 정보 파일 연결 설정
2. DTO와 VO의 알리아스, 매퍼, 데이터 베이스 접속 정보 파일의 경로

# log4j.xml
1. 콘솔 및 로거 파일 설정
2. 로거의 표현 스타일, 형식, 파일의 저장 경로, 최대 용량에 관한 설정

# sample.xml
1. 매퍼
2. 쿼리

---
layout: post
title:  "[spring]mybatis mapping 에러 떄 확인 해야할 것 중 하나"
# date:   2019-05-13 18:34:10 +0700
date:   2020-03-07 00:00:00 +0700
categories: [spring]
---

```java
//SpringConfiguration 설정 파일 중 코드

@Bean(name="sqlSessionFactory")
	public SqlSessionFactory getSqlSessionFactoryBean() throws Exception {
		SqlSessionFactoryBean sqlSessionFactoryBean = new SqlSessionFactoryBean();

		PathMatchingResourcePatternResolver pmrpr = new PathMatchingResourcePatternResolver();
		sqlSessionFactoryBean.setDataSource(dataSource());
		sqlSessionFactoryBean.setConfigLocation(pmrpr.getResource("classpath:spring/mybatis-config.xml"));
		sqlSessionFactoryBean.setMapperLocations(pmrpr.getResources("classpath:sign/*/dao/*Mapper.xml")); //패키지 명에 맞춰 수정

		return sqlSessionFactoryBean.getObject();
	}
```

sqlSessionFactoryBean.setMapperLocations(pmrpr.getResources("classpath:sign/*/dao/*Mapper.xml"));
이부분을 놓치는 경우가 있을 수 있음....

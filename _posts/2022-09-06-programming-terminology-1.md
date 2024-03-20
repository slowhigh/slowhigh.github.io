---
layout: post
title: 프로그래밍 용어 - 1
subtitle: 공부하면서 개념을 명확하게 모르는 용어를 정리해 보자.
excerpt_image: https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/programming-terminology.jpg
categories: Terminology
tags: [AOP, ORM, Boilerplate Code, CQRS, Event Sourcing, SSR, ECMA Script]
---

![banner](https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/programming-terminology.jpg)

오늘은 다양한 프로그래밍 용어에 대해 간단하게 정리해 보겠습니다.

- `AOP (Aspect Oriented Programming, 관점 지향 프로그래밍)`: __Aspect를 사용하여 프로그램의 여러 부분에 걸친 관심사를 모듈화하는 프로그래밍 기술입니다.__ 주요 관심사는 보안, 로깅, 트랜잭션 관리 등이며, 이들을 별도의 모듈로 분리하여 유지보수성을 향상시킵니다.

- `ORM (Object Relational Mapping, 객체 관계 매핑)`: __객체 지향 프로그래밍 언어와 관계형 데이터베이스 간의 데이터를 변환하는 기술입니다.__ 이를 통해 데이터베이스 테이블의 행을 객체로 매핑하고, SQL 쿼리를 사용하여 객체를 데이터베이스에 저장, 검색 및 수정할 수 있습니다.

- `Boilerplate Code (보일러플레이트 코드)`: __반복되는 형식적인 코드로, 개발자가 자주 작성해야 하는 코드를 말합니다.__ 주로 초기 설정이나 템플릿 코드로 사용되며, 실제 비즈니스 로직을 담고 있지 않습니다. 

- `CQRS (Command and Query Responsibility Segregation, 명령과 조회의 책임 분리)`: __데이터 저장소에 대한 읽기 및 업데이트 작업을 구분하는 패턴인 명령과 쿼리의 역할 분리를 의미합니다.__ 애플리케이션에서 CQRS를 구현하면 성능, 확장성 및 보안을 최대화할 수 있습니다. CQRS로 마이그레이션하면 유연성이 생기므로 시스템이 점점 진화하고 업데이트 명령이 도메인 수준에서 병합 충돌을 일으키지 않도록 할 수 있습니다.

- `Event Sourcing Pattern (이벤트 소싱 패턴)`: __시스템의 상태를 변경하는 모든 작업을 이벤트로 기록하고 저장하는 디자인 패턴입니다.__ 이벤트 스트림을 사용하여 시스템의 상태를 추적하며, 이를 통해 시스템의 상태를 재현하고 변경 이력을 추적할 수 있습니다.

- `SSR (Server Side Rendering)`: __웹 애플리케이션의 초기 로딩 시 서버에서 페이지를 렌더링하여 클라이언트에 전송하는 기술입니다.__ 이를 통해 초기 로딩 속도가 개선되며 검색 엔진 최적화(SEO)와 사용자 경험을 향상시킬 수 있습니다. SSR은 React, Vue.js 등의 프레임워크에서도 지원되며, 동적 콘텐츠를 처리하는데 유용합니다.

- `SEO(Search Engine Optimization, 검색 엔진 최적화)`: __웹 사이트가 검색 엔진 결과 페이지(SERP)에서 상위에 표시되도록 최적화하는 프로세스입니다.__ 이를 위해 콘텐츠의 키워드 사용, 링크 구조 최적화, 웹 사이트의 속도 및 사용자 경험 개선 등이 중요합니다. 효과적인 SEO는 웹 사이트의 유기적인 트래픽을 증가시키고 온라인 존재감을 강화하는 데 도움이 됩니다.

- `ECMA Script`: __자바스크립트의 표준화를 위해 ECMA International에서 관리하는 스크립팅 언어 표준입니다.__ 웹 브라우저 및 다양한 환경에서 실행되는 JavaScript의 기본 규격을 정의하며, 자바스크립트 엔진의 개발 및 호환성을 지원합니다. 
---
layout: post
title: 프로그래밍 용어 - 3
subtitle: 공부하면서 개념을 명확하게 모르는 용어를 정리해 보자.
excerpt_image: https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/programming-terminology.jpg
categories: Terminology
tags: []
---

![banner](https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/programming-terminology.jpg)

공부를 하면 할 수록 모르는 용어와 개념을 애매하게 알고 있는 용어들이 많이 발견되는 것 같습니다. 😎

- `cross-cutting concern (크로스커팅 관심사, 횡단 관심사)`: __소프트웨어에서 여러 모듈이나 레이어에 걸쳐서 발생하는 공통 관심사를 의미합니다.__ 이는 애플리케이션의 핵심 기능과는 별도로 관리되며, 로깅, 보안, 트랜잭션 처리와 같은 기능들이 이에 해당합니다. 이를 처리하는 방법으로는 AOP (Aspect-Oriented Programming)가 있습니다.

- `Camel case (카멜 표기법)`: __복합 단어를 구분하기 위해 단어의 첫 글자를 대문자로 표기하는 방법입니다.__ 예를 들어 "camelCase"나 "myVariableName"과 같이 단어의 시작 부분을 제외한 각 단어의 첫 글자는 대문자로 표기됩니다.

- `snake_case (스네이크 표기법)`: __복합 단어를 밑줄('_')로 구분하여 표기하는 방법입니다.__ 예를 들어 "snake_case"나 "my_variable_name"과 같이 사용됩니다.

- `단일 책임 원칙 (SRP, Single Responsibility Principle)`: 소프트웨어 설계 원칙 중 하나로, 클래스나 모듈은 하나의 책임만을 가져야 한다는 원칙입니다. 이는 각각의 클래스나 모듈이 변경되어야 하는 이유를 최소화하여 코드의 응집성을 높이고 유지보수를 용이하게 합니다. 각 구성 요소는 한 가지 기능에만 집중하고 다른 부분과 독립적으로 작동하여 시스템의 복잡성을 줄입니다.
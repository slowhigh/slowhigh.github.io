---
layout: post
title: 프로그래밍 용어 - 2
subtitle: 공부하면서 개념을 명확하게 모르는 용어를 정리해 보자.
excerpt_image: https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/programming-terminology.jpg
categories: Terminology
tags: [DevOps, Endpoint Routing, Sub-Domain Routing, 202 Accepted]
---

![banner](https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/programming-terminology.jpg)

저번 시간에 이어 이번에도 몇 가지 프로그래밍 용어에 대해서 간단하게 정리해 보도록 하겠습니다.

- `DevOps (Development + Operations, 데브옵스)`: __소프트웨어 개발과 정보기술 운영을 결합하는 개발 및 운영 방법론 및 문화입니다.__ 이전에는 개발팀과 운영팀이 각자의 역할을 수행하고 독립적으로 일했던 것과는 대조적으로, 이 두 부분을 하나의 통합적인 프로세스로 병합하고 협업을 강화하는 방식을 나타냅니다.

- `Endpoint Routing`: __네트워크나 시스템에서 메시지, 데이터, 요청 등이 어디로 전송될지 결정하는 메커니즘입니다.__ 이는 일반적으로 네트워크 통신에서 발생하며, 웹 서비스, 마이크로서비스 아키텍처, 컴퓨터 네트워크 등에서 사용됩니다. 엔드포인트는 특정 서비스 또는 리소스에 접근할 수 있는 주소나 위치를 나타냅니다.

- `Sub-Domain Routing`: __하나의 도메인에 여러 서브도메인을 할당하여 각 서브도메인에 해당하는 서비스 또는 리소스로 요청을 라우팅하는 메커니즘입니다.__ 이를 통해 서브도메인 단위로 서로 다른 애플리케이션 또는 기능을 호스팅할 수 있으며, 관리와 확장이 용이합니다. 대표적으로 DNS나 웹 서버 설정에서 서브도메인을 지정하여 트래픽을 분배합니다.

- `비확정적 상태 코드(202 Accepted)`: __클라이언트의 요청이 서버에 의해 수신되었으며, 처리되지 않았지만 나중에 처리될 것임을 나타냅니다.__ 이 상태 코드는 비동기 작업을 지원하고, 클라이언트에게 요청의 성공을 알리면서 작업 완료를 기다리는 시간을 제공합니다. 클라이언트는 나중에 작업 결과를 확인하기 위해 추가 요청을 보낼 수 있습니다.
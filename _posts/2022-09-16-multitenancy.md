---
layout: post
title: Multi-tenancy Architecture
subtitle: 아키텍처를 알아야 구조가 보인다.
excerpt_image: https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/multitenancy.png
categories: Architecture
tags: [Multitenancy, multi-tenant]
---

![banner](https://cdn.jsdelivr.net/gh/slowhigh/slowhigh.github.io@main/assets/images/multitenancy.png)

`Multi-tenancy Architecture`하나의 소프트웨어 시스템이 여러 개의 `Tenant`(사용자 그룹 또는 고객)를 지원하는 방법론입니다. 각 `Tenant`는 독립적으로 자신의 데이터, 설정, 사용자 인터페이스 등을 가질 수 있지만, 하나의 소프트웨어 인스턴스를 공유하여 리소스를 효율적으로 활용할 수 있습니다. 이 방법론은 3가지 모델로 나뉠 수 있습니다.

1. 인스턴스 복제 모델
- 각 `Tenant`마다 별도의 서버와 데이터베이스를 제공하여 단순하게 확장 가능한 구조입니다.
- 개발 및 성능 측면에서 우수하지만 비용과 확장성에 제약이 있을 수 있습니다.

2. 데이터베이스 분리 모델
- 모든 `Tenant`가 단일 서버를 공유하며 각각의 데이터베이스를 사용합니다.
- 성능은 인스턴스 복제보다 약간 떨어질 수 있지만, 유휴 상태에서 비용 절감이 가능합니다.
- 그러나 여전히 각 `Tenant`마다 별도의 데이터베이스를 필요로 하므로 확장성에 제약이 있습니다.

3. 스키마 분리 모델:
- 단일 데이터베이스 내에서 각 `Tenant`의 데이터를 논리적으로 분리합니다.
- 성능과 비용 측면에서 우수하며, 데이터의 논리적 분리를 통해 격리를 달성할 수 있습니다.

스키마 분리 모델이 이상적으로 보이지만, 실제로는 개발자의 실수로 인한 문제가 없고 논리적 분리를 통해 격리를 달성한다는 장점을 제공합니다. 이렇게 `Multi-tenancy Architecture`을 적용할 때는 각 모델의 장단점을 고려하여 적절한 모델을 선택하는 것이 중요합니다.
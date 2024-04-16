---
layout: post
title: n값을 이진법으로 변환하기
subtitle: 코드는 사소하나 속도는 심각하다.
excerpt_image: https://camo.githubusercontent.com/89e3fc81036629031e787c8d09cb08bb50993b1b4c6f6ecd72e4a7c41f398c5b/68747470733a2f2f676f6c616e672e6f72672f646f632f676f706865722f6669766579656172732e6a7067
categories: Code
tags: [Go, golang]
---

![banner](https://camo.githubusercontent.com/89e3fc81036629031e787c8d09cb08bb50993b1b4c6f6ecd72e4a7c41f398c5b/68747470733a2f2f676f6c616e672e6f72672f646f632f676f706865722f6669766579656172732e6a7067)

golang에서 n값을 이진법으로 변환할 때 사용하는 라이브러리를 비교해 보겠습니다.

`strconv.FormatInt(int64(n), 2)`와 `fmt.Sprintf("%b", n)`은 모두 정수를 2진수 문자열로 변환하는 함수이지만, 성능 측면에서 몇 가지 주요 차이점이 있습니다.

1. 변환 방식:
strconv.FormatInt: 문자열 버퍼를 직접 사용하여 변환합니다. 이는 메모리 할당 및 해제 과정을 줄이고 성능 향상에 도움이 될 수 있습니다.
fmt.Sprintf: sprintf 함수를 내부적으로 사용하여 변환합니다. sprintf 함수는 다양한 형식 문자열을 처리하도록 설계되었으므로 strconv.FormatInt보다 더 복잡하고 느릴 수 있습니다.

2. 정밀도:
strconv.FormatInt: 변환된 문자열의 정밀도를 제어할 수 있습니다. 예를 들어, strconv.FormatInt(n, 10)은 n을 10자리 2진수 문자열로 변환합니다.
fmt.Sprintf("%b", n): 정밀도를 자동으로 설정합니다. 기본적으로 n의 비트 수만큼의 자리가 사용됩니다.

3. 속도 비교:
일반적으로 strconv.FormatInt는 fmt.Sprintf("%b")보다 빠르다고 알려져 있습니다. 특히, 변환해야 하는 정수가 크거나 정밀도가 중요한 경우 더욱 그렇습니다. 하지만, 실제 속도 차이는 여러 요인에 따라 달라질 수 있습니다.
- 정수 크기: 정수가 클수록 strconv.FormatInt와 fmt.Sprintf("%b") 모두 속도가 느려집니다.
- 사용 빈도: 함수를 자주 사용하는 경우, 미리 컴파일된 코드가 생성되어 속도가 향상될 수 있습니다.
- Go 버전: 최신 버전의 Go는 성능 개선을 포함할 수 있습니다.

strconv.FormatInt와 fmt.Sprintf("%b") 중 어느 것이 더 빠른지는 상황에 따라 다릅니다. 정확한 성능 비교를 위해서는 실제 코드에서 두 함수를 모두 사용하여 테스트하는 것이 좋습니다. 또한, Go의 공식 문서 및 성능 벤치마킹 자료를 참고하는 것도 도움이 될 수 있습니다.
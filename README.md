# ducky

> 덕키 다자인 시스템

ducky 는 3개로 구성된 duckie 의 디자인 시스템 입니다.

---

## UI

TODO



## Writing

... TODO



## Compose

1. Modifier 첫 번째 인자 및 default argument 설정 필수

> Composable 의 유연한 확장성을 위함

```kotlin
@Composable
fun Ducky(
    modifier: Modifier = Modifier // 필수, 무조건 첫 번째 인자 및 default argument 로 돼야 함
)
```

2. List 대신 ImmutableList 사용

> Immutable 을 위함

```kotlin
@Composable
fun Ducky(
    lists: ImmutableList<String>
)
```

a. named-argument 필수? (단, 일부 예외 있을 수 있음)

b. 모든 인자는 new-line 으로 배치? (단, 일부 예외 있을 수 있음)

... TODO



## Generic

1. 상단에 Copyright 2번 감지

```
/*
 * Copyright 1
 */

/*
 * Copyright 2
 */
 
 // Error!
```

a. 인자 끝 항상 `,` 으로 끝낼지?

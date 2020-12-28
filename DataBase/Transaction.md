# 트랜잭션 이론

## 트랜잭션
정의 : 데이터베이스의 상태를 변환시키는 하나의 논리적 기능을 수행하기 위한 작업의 단위 또는 한꺼번에 모두 수행되어야 할 일련의 연산들을 의미<br>
- 사용자의 질의를 처리할 때 트랜잭션 단위로 처리한다.
- 즉, 트랜잭션이란 사용자의 질의 연산의 집합이다.

## 트랜잭션의 ACID 특성

### 1. Atomicity (원자성)
데이터베이스에 전부 반영이 되거나, 전부 반영이 되지 않아야 한다. (all or nothing)

### 2. Consistency (일관성)
일관성을 유지해야 한다.
- 명시적으로 선언한 키들은 정해진 제약을 따라야 한다.<br>
- 묵시적인 제약 또한 존재<br>

### 3. Isolation (독립성,격리성,고립성)
각 트랜잭션은 다른 트랜잭션의 수행을 알지 못한체 정상적으로 작동되어야 한다. 

### 4. Durability (영속성)
트랜잭션이 성공적으로 수행되었다면, 그 변화는 시스템이 망가져도 데이터베이스에 적용되어야 한다.
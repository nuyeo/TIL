연결리스트

---

## 1. 연결 리스트(Linked List)
![image](https://github.com/user-attachments/assets/caf22f97-725f-4fa3-bdbb-c9db0d64c0ef)


- '데이터(값) + 다음 노드를 가리키는 포인터'로 이루어진 노드(node)들이 순차적으로 연결된 구조
- 값 + 주소가 한 쌍으로 구성

---

## 2. 특징
- 메모리에 있는 데이터의 물리적 배치 사용 X (인덱스 X, 참조 시스템 사용) -> 연속된 메모리에 저장 X
- 단일/이중/원형 형태가 있음
- 포인터 직접 관리 필요
- 느린 접근
- 빠른 삽입/삭제 (python의 `collections.deque`가 내부적으로 이중 연결 리스트 기반 -> 빠른 양방향 삽입/삭제)
- 포인터 저장용 메모리가 추가로 필요

---

## 3. 연결 리스트 구조
- 단일 연결 리스트 (Singly Linked List): `Head → Node1 → Node2 → Node3 → NULL`

- 이중 연결 리스트 (Doubly Linked List): `NULL ← Node1 ⇄ Node2 ⇄ Node3 → NULL`

- 원형 연결 리스트 (Circular Linked List): `Node1 → Node2 → Node3 → (다시 Node1)`

---

## 4. 주요 연산 시간 복잡도
| 연산 | 시간 복잡도 |
|------|--------------|
| 접근 (인덱스) | O(n) |
| 탐색 (순차 검색) | O(n) |
| 삽입/삭제 (노드 위치 알고 있을 경우) | O(1) |

---

## 5. 언제 사용할까?
- 데이터의 크기가 자주 바뀌는 경우
- 앞/중간에 자주 삽입/삭제가 일어나는 경우
- 큐, 스택 자료구조 구현

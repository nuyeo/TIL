덱

---

## 1. 덱(Deque, Double Ended Queue)
![image](https://github.com/user-attachments/assets/e04fd09e-d5fe-4c32-a56c-30517fddd74b)



- 양쪽(앞, 뒤)에서 모두 삽입/삭제가 가능한 큐
- 스택+큐의 특성을 모두 가진 구조

---

## 2. 특징
- 모든 연산이 O(1)
- 삽입, 삭제 빠름, 양방향에서 가능
- 중간 데이터 접근 및 인덱스 접근은 비효율적
- 스택, 큐 모두 대체 가능

---

## 3. 주요 연산 시간 복잡도
| 연산 | 시간 복잡도 |
|------|--------------|
| 삽입 (`append`, `appendleft`) | O(1) |
| 삭제 (`pop`, `popleft`)| O(1) |
| 인덱스 접근 | O(n) |

---

## 4. 언제 사용할까?
- 양방향 탐색 (회전 큐, 양쪽 조건 우선순위 처리)
- 슬라이딩 윈도우

---

## 5. 덱 vs 큐 vs 스택

| 자료구조 | 삽입 방향 | 삭제 방향 | 주요 특징 |
|----------|------------|-------------|-------------|
| 스택 | 한쪽 (뒤) | 한쪽 (뒤) | LIFO |
| 큐 | 뒤 | 앞 | FIFO |
| 덱 | 앞/뒤 | 앞/뒤 | 양방향 가능 (스택+큐) |

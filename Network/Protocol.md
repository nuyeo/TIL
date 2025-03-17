### 📌 프로토콜 (Protocol)

---

## 1. 프로토콜이란?
- 통신을 위해 정해진 규칙과 규약의 집합.
- 서로 다른 시스템이 데이터를 주고받을 때 동일한 방식으로 이해할 수 있도록 정의됨.
- 하드웨어 및 소프트웨어 간의 원활한 통신을 보장함.

---

## 2. 프로토콜의 주요 요소
1. **구문 (Syntax)**  
   - 데이터의 형식, 구조, 부호화 방식 정의.
2. **의미 (Semantics)**  
   - 송신자와 수신자가 어떻게 데이터를 해석할지에 대한 규칙.
3. **타이밍 (Timing)**  
   - 데이터 전송 속도, 순서, 흐름 제어 등의 동기화 방식.

---

## 3. 네트워크 계층별 프로토콜
### 1️⃣ 물리 계층 (Physical Layer)
- 기능: 실제 데이터 전송 (전기 신호, 빛 신호, 무선 신호 등).
- 예시: Ethernet(IEEE 802.3), USB, Bluetooth, Wi-Fi(IEEE 802.11)

### 2️⃣ 데이터 링크 계층 (Data Link Layer)
- 기능: MAC 주소 기반 데이터 전송, 오류 검출 및 흐름 제어.
- 예시: Ethernet, PPP(Point-to-Point Protocol), ARP(Address Resolution Protocol)

### 3️⃣ 네트워크 계층 (Network Layer)
- 기능: IP 주소 기반 데이터 전송, 경로 설정 (라우팅).
- 예시: IP(Internet Protocol), ICMP(Internet Control Message Protocol), OSPF, BGP

### 4️⃣ 전송 계층 (Transport Layer)
- 기능: 포트 기반 데이터 전송, 오류 복구 및 흐름 제어.
- 예시: TCP(Transmission Control Protocol), UDP(User Datagram Protocol)

### 5️⃣ 세션 계층 (Session Layer)
- 기능: 통신 세션(연결) 관리.
- 예시: TLS(Transport Layer Security), NetBIOS

### 6️⃣ 표현 계층 (Presentation Layer)
- 기능: 데이터 인코딩, 압축, 암호화.
- 예시: SSL(Secure Sockets Layer), JPEG, MPEG, ASCII, TLS

### 7️⃣ 응용 계층 (Application Layer)
- 기능: 사용자와 직접 상호작용하는 프로토콜.
- 예시: HTTP, FTP, SMTP, DNS, SSH

---

## 4. 주요 프로토콜 비교

| 프로토콜 | 계층 | 특징 |
|----------|------|------|
| **TCP** | 전송 계층 | 연결 지향, 신뢰성 보장, 순서 보장 |
| **UDP** | 전송 계층 | 비연결형, 빠른 속도, 신뢰성 보장 X |
| **IP** | 네트워크 계층 | 패킷 기반 주소 지정 및 전송 |
| **HTTP** | 응용 계층 | 웹 통신, 상태 비유지(Stateless) |
| **HTTPS** | 응용 계층 | HTTP + TLS로 보안 강화 |
| **FTP** | 응용 계층 | 파일 전송 프로토콜 |
| **DNS** | 응용 계층 | 도메인 이름을 IP 주소로 변환 |

---

## 5. TCP vs UDP
| 항목 | TCP | UDP |
|------|----|----|
| 연결 방식 | 연결 지향(Connection-oriented) | 비연결(Connectionless) |
| 신뢰성 | 데이터 손실 방지, 순서 보장 | 신뢰성 없음, 빠른 전송 |
| 속도 | 상대적으로 느림 | 빠름 |
| 예시 | HTTP, HTTPS, FTP, SMTP | DNS, VoIP, 스트리밍 |

# [ 1주차_Network_JYT ]

Status: 완료
날짜: 2025/06/13 → 2025/06/14
선택: 1주차
작성자: 전영태

# **네트워크의 큰 그림**

### **1. 네트워크란 무엇인가?**

- **노드(Node)**: 네트워크에 연결된 컴퓨터, 서버, 공유기 같은 장비
- **간선(Edge)**: 노드를 연결하는 유선/무선 통신 매체
- 네트워크는 **그래프 구조**로 볼 수 있음 (노드와 간선의 연결)

---

### **2. 네트워크 구성 요소**

| **요소** | **설명** |
| --- | --- |
| **호스트(Host)** | 네트워크 내에서 데이터를 최초로 송신하거나 수신하는 장비 (ex. 노트북, 서버 등) |
| **클라이언트/서버** | 요청을 보내는 쪽이 클라이언트, 응답을 보내는 쪽이 서버 |
| **중간 노드** | 스위치, 라우터, 공유기 등 - 데이터를 중계하고 전달 |

---

### **3. 네트워크의 유형**

| **분류** | **설명** |
| --- | --- |
| **LAN (근거리 네트워크)** | 집, 학교, 회사처럼 일정 공간 내의 네트워크 |
| **WAN (광역 네트워크)** | LAN과 LAN을 연결한 큰 규모 네트워크 (ex. 인터넷) |
| **ISP (인터넷 서비스 제공자)** | KT, SK브로드밴드 등이 WAN을 관리 |

---

### **4. 데이터 전송 방식**

- **패킷(Packet)**: 데이터를 잘게 나눠 보내는 단위
    - 구성: 헤더(Header), 페이로드(Payload), (선택적) 트레일러
- **전송 방식**
    - 유니캐스트: 1:1 전송
    - 브로드캐스트: 1:전체 전송
    - 멀티캐스트: 1:그룹 전송
    - 애니캐스트: 1:가장 가까운 1인 전송

---

### **5. 주소 체계**

| **주소 종류** | **설명** |
| --- | --- |
| **IP 주소** | 네트워크 상에서 장비를 식별 |
| **MAC 주소** | LAN 내부에서 장비를 식별 (하드웨어 고유 주소) |

---

### **6. 프로토콜 (Protocol)**

- 통신을 위한 규칙
- 주요 프로토콜:
    - **IP**: 주소 지정 및 패킷 전달
    - **ARP**: IP ↔ MAC 매핑
    - **TCP / UDP**: 신뢰성 vs 속도
    - **HTTP / HTTPS**: 웹 통신
    - **DNS**: 도메인 이름을 IP로 변환

---

### **7. 네트워크 참조 모델**

| **OSI 7계층** | **TCP/IP 4계층** | **역할 요약** |
| --- | --- | --- |
| 응용계층 | 응용계층 | 사용자 서비스 (HTTP, DNS 등) |
| 표현계층 | (응용계층 포함) | 인코딩, 암호화 |
| 세션계층 | (응용계층 포함) | 연결 관리 |
| 전송계층 | 전송계층 | 포트 사용, TCP/UDP |
| 네트워크계층 | 인터넷계층 | 라우팅, IP |
| 데이터링크계층 | 네트워크 엑세스계층 | MAC 주소 기반 통신 |
| 물리계층 | 네트워크 엑세스계층 | 전기 신호, 케이블 등 |

※ TCP/IP 모델은 구현 중심, OSI는 개념 중심

---

### **8. 캡슐화와 역캡슐화**

- **캡슐화(Encapsulation)**: 송신 측에서 데이터에 계층별 헤더를 붙여 전송
- **역캡슐화(Decapsulation)**: 수신 측에서 계층별로 헤더를 제거하고 원래의 데이터를 복원

---
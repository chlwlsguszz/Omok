# Omok (오목) 🎮  
Java 기반 네트워크 오목 게임

---

## 📌 프로젝트 개요
- **과목**: 네트워크 프로그래밍  
- **프로젝트 유형**: 텀 프로젝트  
- **게임명**: 오목 (Omok)  
- **개발 언어**: Java  
- **구성**: Client / Server 구조의 네트워크 게임  

---

## 👥 팀원 및 역할
| 이름 | 역할 |
|----|----|
| 최진현 | 방 생성/참여, 채팅, 프로필 이미지, 무르기, 방장 기능 |
| 김성훈 | 오목 기본 로직, 타이머, 네트워크 진행, 관전/복기 |

---

## 🎯 주요 기능

### 🔐 로그인 & 프로필
- 로그인 기능
- 프로필 이미지 선택  
  - `profileImg` 폴더 내 이미지 중 선택

### 🏠 방 관리
- 방 생성 / 입장 / 종료
- 인원 설정
  - 2인 (1:1)
  - 3인 (1:1:1)
  - 4인 (2:2)
- 방 목록 및 방 내 유저 리스트 관리

### 💬 채팅
- 전체 채팅
- 방별 채팅
- 방장 기능
  - 강제 퇴장
  - 채팅 금지

### ♟️ 게임 플레이
- 오목 기본 룰
- 턴 제한 시간: **30초**
- 시간 초과 시 자동 턴 넘김
- **무르기 기능**
  - 투표 방식
  - 전원 찬성 시 적용

### 👀 관전 & 복기
- 방 인원 초과 시 관전자 입장
- 이전 / 다음 버튼으로 복기
- 관전자 훈수 기능 (1회)

### 🔄 멀티 게임
- 여러 게임 동시 진행 가능

---

## 🧩 시스템 구조

### 시스템 구성도
- Java Game Server
- 다수의 Java Game Client
- ClientService Thread 기반 다중 접속 처리

### 시스템 흐름
1. Client → Server 연결 요청
2. `gameMsg` 객체 송수신
3. 프로토콜 내용에 따라 동작 처리
4. 화면 출력 및 게임 진행

---

## 📡 프로토콜
- `gameMsg` 객체 기반 통신
- 명령/상태 중심 프로토콜 설계
- 서버에서 메시지 해석 후 클라이언트 동작 제어

---

## 🖥️ 실행 화면
![Image](https://github.com/user-attachments/assets/505f8e03-f94f-4f6a-8dda-49fa75d8fc60)
![Image](https://github.com/user-attachments/assets/e19aca86-8a53-4260-aa9e-dc7b24803ab2)
![Image](https://github.com/user-attachments/assets/20cb2339-7fa4-432c-8347-5d63b42adb4f)
![Image](https://github.com/user-attachments/assets/1835df06-b48a-4677-9c83-f325af3bd83c)

---

## 🎥 시연 영상
[ 링크 ](https://youtu.be/mHga5RdikNg)

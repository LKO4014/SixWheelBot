# SixWheelBot
라즈베리파이5를 이용한 배달로봇 프로젝트

<img alt="fullfaceImage" src="https://github.com/user-attachments/assets/fedf318a-e128-4af0-88bf-a3dff63528e7" width="35%" />
<img alt="wildImage" src="https://github.com/user-attachments/assets/15cec6b3-73db-4152-872e-13a3af4c80c0" width="55%" />

---

## 프로젝트 개요
### 문제 정의
- 기존 배달 로봇들의 구매 비용 + 개발비 + 유지비용 ... : 서비스 비용은 단 돈 1,000원..?
- 배달 성능의 문제 : 차량과 부딪히고, 인파 속에서 길을 헤매고..

### 프로젝트 컨셉
좀 더 경제적이고 적은 부품으로 다양한 지형지물을 극복하는 배송 로봇을 만들어보자!

### 서비스 플로우
<img width="1535" height="795" alt="Image" src="https://github.com/user-attachments/assets/e6adb43e-b951-4177-8bdc-4b5be9c52f1c" width="45%" />

## 시스템 플로우
<img width="877" height="322" alt="Image" src="https://github.com/user-attachments/assets/c79f2215-debb-4d19-8cfa-840cc8255f7d" width="45%" />

## 결과
## 결과

<details>
  <summary><b>⚙️ 모터 제어 (Motor Control Module)</b></summary>
  <br>
  <p align="center">
    <img alt="gif1" src="https://github.com/user-attachments/assets/7984b750-42b8-42bb-96d6-06b51aab6f72" width="45%" />
    <img alt="gif2" src="https://github.com/user-attachments/assets/19eb5cf9-907c-4f40-b85a-484fbe17b21f" width="45%" />
  </p>
</details>

<details>
  <summary><b> 적재함 평형 유지 (Equilibrium Module)</b></summary>
  <br>
  <p align="center">
    <img src="https://github.com/user-attachments/assets/84587b8f-13cd-401b-b630-ed0175b0b64c" width="90%" alt="평형 유지">
  </p>
</details>

<details>
  <summary><b> 주행 명령 (Motor Command Module)</b></summary>
  <br>
  <p align="center">
    <img src="https://github.com/user-attachments/assets/5cb5c91d-f478-452c-9140-5a7e7bb309fe" width="90%" alt="주행 명령" />
  </p>
</details>

<details>
  <summary><b> 장애물 감지 (Lidar Module)</b></summary>
  <br>
  <p align="center">
    <img alt="장애물 감지" src="https://github.com/user-attachments/assets/2a9083ec-4eb8-4aca-a052-4ea40fbaef66" width="90%" />
  </p>
</details>

<details>
  <summary><b> 인도 인식</b></summary>
  <br>
  <p align="center">
    <img alt="인도 인식" src="https://github.com/user-attachments/assets/a28a5e3a-6a2e-4df6-978a-bf859e00b5a5" width="90%" />
  </p>
</details>

<details>
  <summary><b> 험지 극복</b></summary>
  <br>
  <p align="center">
    <img src="https://github.com/user-attachments/assets/d9fc3db1-43ab-4e3f-b9c2-1419492d6583" width="90%" alt="장애물 극복" />
  </p>
</details>



## 📁 SixWheelBot 디렉토리 구조

```plaintext

SixWheelBot/
├── AI_Server/              # AI 모델 서버 통신 모듈
├── Config/                 # 설정 파일
├── LiDAR_Server            # LiDAR 센서 데이터 수집 및 전송 모듈
|   ├── YDLidar-SDK/        # YDLiDAR SDK 라이브러리 파일
├── Main/                   # 배달 로봇 통합 모듈
|   ├── Arduino/            # 아두이노 
│   ├── Communication/      # 통신 모듈
│   ├── GPS/                # GPS 모듈, Tmap 연동 모듈
│   │   └── lib/            # GPS 모듈관련 라이브러리 파일
│   ├── LiDAR/              # LiDAR 센서 데이터 수신 모듈
│   ├── Motor/              # Arduino 기반 Motor 제어 모듈
│   └── Vision/             # 이미지 추출 및 AI 서버 전송 모듈
├── Web/                    # 웹 서버 및 배달 로봇 통신 모듈
│   ├── web_project         # Node.js + react 기반 웹 서버
└───└── serer.py            # 웹 서버 <> 배달 로봇 통신 모듈
```

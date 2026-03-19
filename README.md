# SixWheelBot
라즈베리파이5를 이용한 배달로봇 프로젝트

<img alt="fullfaceImage" src="https://github.com/user-attachments/assets/fedf318a-e128-4af0-88bf-a3dff63528e7" width="35%" />
<img alt="wildImage" src="https://github.com/user-attachments/assets/15cec6b3-73db-4152-872e-13a3af4c80c0" width="55%" />

## 육륜이 시스템 구조도
<img width="877" height="322" alt="Image" src="https://github.com/user-attachments/assets/c79f2215-debb-4d19-8cfa-840cc8255f7d" width="45%" />

## 결과
<detail>
  <summary>
    육륜이 회전 ( -60 degrees & 90 degrees)
    <img alt="gif1" src="https://github.com/user-attachments/assets/7984b750-42b8-42bb-96d6-06b51aab6f72" width="45%" />
    <img alt="gif2" src="https://github.com/user-attachments/assets/19eb5cf9-907c-4f40-b85a-484fbe17b21f" width="45%" />
    적재함 평형 유지
    ![Image](https://github.com/user-attachments/assets/84587b8f-13cd-401b-b630-ed0175b0b64c)
  </summary>
  
</detail>


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

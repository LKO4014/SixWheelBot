# SixWheelBot
라즈베리파이5를 이용한 배달로봇 프로젝트

모듈 별 개별 디렉토리에 작업

<img width="273" height="529" alt="Image" src="https://github.com/user-attachments/assets/fedf318a-e128-4af0-88bf-a3dff63528e7" /> 
<img width="877" height="322" alt="Image" src="https://github.com/user-attachments/assets/c79f2215-debb-4d19-8cfa-840cc8255f7d" />

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

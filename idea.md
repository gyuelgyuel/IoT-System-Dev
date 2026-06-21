# Idea List
## 아이디어 수집
### 스마트 전등
1. 아이디어 수집
  - 핸드폰 어플과 연결하여, 전등 제어 시스템 만들기
  - 알람 시간과 연동하여 전등 켜기
  - 핸드폰 뮤직에 맞춰 다양한 색 전등 변화
2. 전등 종류
  - 다운 조명
    - 정전압(다수), 정전류(빛의 움직임이 부드러움)
      - 참고 링크 : https://www.youtube.com/watch?v=CIcU6zKT-eQ
  - 라인 조명
    - 천장 매립 혹은 직부 형태로 사용
    - LED 스트립/바, RGB 컬러 제품이 있음
  - 면/엣지 조명
  - 그릴/그룹 라이트

## HW
### 구성
1. PCB 메인보드 설계 각 모듈, 인터페이스 배치 및
- MCU 선정(PWM 개수, CAN/Ethernet 지원 여부, ADC 등을 고려)
- 전원공급설계 (모터 전원 때문에 MCU 전원이 흔들려서는 안됨, 전원분리는 가격 및 소비전력 고려하여 선정)
- motor driver 설계 (Servo - PWM / Stepper - Driver IC / BLDC - 3상 Driver IC)
- 보호 회로 설계
- 통신회로 (CAN/Ethernet/RS485)
  - CAN : 종단 저항 필요, differential 배선 길이 맞추기, TVS/Common Mode Choke를 넣어서 CMRR 개선
  - RS485 : Idle 상태 Floating 방지용 Bias Register 적용
- 인터페이스에 따른 배선 설계 (UART:TX-RX 교차 연결 및 GND 공유 등 / I2C:pull up 필요, differential I2C 활용 등 / SPI: slave 가까이 배치, clock, gnd return, trace 길이 등 고려)
2. 전원 공급 장치 (SMPS, 안정기)
3. 스트립 드라이버
   - 조명 그룹별 제어장치
   - 그룹 개수만큼 필
4. 
## SW
## 보안
### 회로 안전
### 해킹 보안

## 로봇 공학
### 기술/연구 분야
1. SLAM
2. Path Planning
3. Estimation
4. Control
5. Computer Vision

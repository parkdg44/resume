# 이력서

## 소개

<img src="images/박동규.jpg" width="200" height="280"/>

- 이름: 박동규 
- 전공: Mobile Robot Navigation
- 메일: parkdg44@naver.com
- 깃허브 링크: https://github.com/parkdg44/resume

## 학력
- 서울과학기술대학교 기계설계로봇공학과 석사 과정 (2020.03 ~ 2022.02)
    - 졸업논문: [3차원 객체 인식과 속도 피드백을 통한 주행 로봇의 자율 위치 추종 제어 기법](http://www.riss.kr/search/detail/DetailView.do?p_mat_type=be54d9b8bc7cdb09&control_no=72c6a0a76ee12ab0ffe0bdc3ef48d419&outLink=N)
- 서울과학기술대학교 기계시스템디자인공학과 (2014.03 ~ 2020.02)

## 기술 스택

### Python
- Pytorch: Model Inference / Pipelining
- FMPy: FMI 활용 경험
    - FMI(Functional Mock-up Interface) \
    : 시뮬레이션 툴 간 협업을 위해 제안된 동적 시스템 모델 인터페이스.
- opencv: 영상 처리 활용 경험 
    - Morphological Transformations, ...

### C++
- MCU Firmware Development
    - Mbed OS, STM32duino, ...

### Robotics & Control
- Full State Feedback: [Reaction Wheel 제어 경험](https://github.com/parkdg44/NANOLAB/tree/master/reaction_wheel)
- 각종 신호 처리 필터 활용 경험 
    - LPF, HPF, Complementary Filter, Kalman Filter, ...
- Mobile Robot
    - Dead Reckoning, Feedback Control, ...
- Perception: [3D Object Detection(YOLOv5+DBSCAN)](https://github.com/parkdg44/Platform_ROS2_ws/blob/main/workspaces/self_drive_ws/src/vision/detection_2d)

### ROS 1 & 2
- Workspace 구성 및 배포 경험
    - [자율 청소 로봇](https://github.com/parkdg44/Platform_ROS2_ws), [실내 자율 주행 AGV 프로젝트](https://github.com/parkdg44/NANOLAB/tree/master/AGV) 등
- Nav 1 / 2 활용 경험
    - Laser Scan, Odometry 등 패키지 활용에 필요한 각종 데이터 Pipelining
    - 로봇에 적합한 Behavior Tree 작성 경험
- ROS1 -> ROS2 패키지 Porting 경험
    - [ira_laser_tools /  laserscan_multi_merger 패키지 포팅 및 활용](https://github.com/parkdg44/Platform_ROS2_ws/blob/main/workspaces/self_drive_ws/src/tools/laserscan_merger)

## 전공 관련 프로젝트 이력

- [실내 자율주행 청소 로봇 시스템 개발](https://github.com/parkdg44/Platform_ROS2_ws)
    - 설명: 기존의 실내 청소 로봇의 한계를 극복하기 위해 자율주행 및 청소, 보행자 
인식, GUI 인터페이스 등을 탑재한 지능형 자율 청소 로봇 시스템을 개발함.
    - 주관: (주)제우스로보틱스
    - 기간: 2021.06.01 ~ 2021.12.31
    - 역할
        - ROS2 Workspace 구성 및 배포
        - 각종 센서를 결합하여(IMU, 모터 엔코더, T265 등) Localization 구현
        - T265(VIO) 속도 추정 결과를 활용한 피드백 제어 기술 구현
        - Nav 2 기반 자율 주행 / 자율 청소 기술 구현
        - 객체 인식(YOLOv5)과 군집화 알고리즘(DBSCAN)을 결합한 3D 객체 인식 기술 구현
        - QT 기반 통합 GUI 인터페이스 구현
        - 로봇 팔 제어 기술과 3D 객체 인식 기술을 이용한 엘리베이터 버튼 조작 기능 구현
        - 3D 객체 인식 기술을 활용한 보행자 인식 및 대응 기술 구현
        - 시나리오 별 흐름도 구상 및 구현
        - Project Management (시스템 구상, 주관업체 응대, 인계자료 작성 등)
    - 주요 성과
        - 속도 추종 제어: 약 +-0.18m/s 속도, 10% 슬립을 가정했을 때, 안정화 구간에서 평균 2%정도의 오차율을 보임
        - 3D 객체 인식: 약 1.8m 정도의 구간에서 평균 7.6cm의 측정 오차, 8~10 FPS
        - 업체에서 요구한 자율주행, 자율청소, 보행자 인식 및 대응, 엘리베이터 버튼 조작 기능에 대해 문제없이 동작하는 것을 실험으로 확인함
        - 특수한 로봇 플랫폼(매카넘 휠)의 시스템 모델링 경험 습득
        - 딥러닝 모델 IO Pipelining 경험 습득

- [ROS 기반 실내 자율 주행 AGV 개발](https://github.com/parkdg44/NANOLAB/tree/master/AGV)
    - 설명: 학사 캡스톤 디자인으로 진행했던 프로젝트로 물류 센터 무인화를 위해 
상자 분류, 목표 설정, 자율주행 기능을 수행하는 AGV를 개발함.
    - 주관: 서울과학기술대학교
    - 기간: 2019.03.01 ~ 2019.12.31
    - 역할
        - MCU 펌웨어 개발 및 IMU, 엔코더 센서를 결합하여 Localization 구현
        - Navigation 기반 자율 주행 기술 구현
        - ROS 기반 통합 시스템 및 전체 시퀀스 동작 구현
    - 주요 성과
        - 로봇 시스템 통합 경험, ROS 사용 경험 습득

- 가상환경 기반 자율주행차 시뮬레이터 개발
    - 설명: 기존의 상용 차량 시뮬레이터의 가격이 부담되는 중소기업을 대상으로 
오픈소스 기반의 차량 시뮬레이터를 개발함.
    - 주관: 한국기계연구원
    - 기간: 2021.04.22 ~ 2021.06.22
    - 역할
        - Project Management (시스템 구상, 주관업체 응대, 인계자료 작성 등)
        - FMI 인터페이스 기반 차량 모델 동적 해석 소프트웨어 개발
        - Unity를 활용한 차량 3D 시각화 소프트웨어 개발
    - 주요 성과
        - 차량 모델링 해석 경험, 주관업체 응대 요령 습득
        - 시뮬레이션 툴에서 FMU 추출 및 프로그램 적용 경험 습득

## 연구 과제 이력

- 태양광발전 설비 유지보수용 고장 진단 청소 복합 임무 로봇 개발
    - 설명: 태양광 발전 효율성을 증대하기 위해 태양광 발전 패널 청소 업무를 수행하는
로봇 시스템을 개발함.
    - 주관: (주)에코센스
    - 기간: 2020.03.01 ~ 2020.12.31
    - 역할
        - 로봇 관제 소프트웨어 개발
        - 태양광 패널 내에서의 위치 및 자세 추정 알고리즘 개발
    - 주요 성과
        - 로봇의 9축 자세 추정 및 센서 퓨전 경험 습득
    
- 호흡기 및 기체분석 장비 모니터링 시스템 개발 \
  호흡기체 검사장치 및 기능결함 감지 장치 시제품 제작
    - 설명: 스쿠버 다이버의 장비 결함으로 인한 사고가 빈번하게 발생함에 따라 스쿠버
장비의 결함을 진단하고 대응할 수 있는 검사 시스템을 개발함.
    - 주관: 스쿠버엔지니어링
    - 기간: 2020.07.01 ~ 2021.12.31 / 2021.04.01 ~ 2021.12.31
    - 역할
        - 공기통 내부 기체 검사장치 소프트웨어(C#) 개발
        - 스쿠버 호흡기 안전 검사 장치 소프트웨어(C#) 개발 및 추가 보완
        - Project Management(2021.04 ~ 2021.11) 업무 수행
    - 주요 성과
        - 각종 센서 활용 경험, 업체 응대 및 프로젝트 관리 요령 습득
    
- 건설현장 안전보호구 스마트 관리 시스템 개발
    - 설명: 건설현장 내에서 작업자들의 현장 출입 관리 및 위험지역 노출 여부를
모니터링하기 위해 관제 시스템을 개발함.
    - 주관: (주)그인토탈
    - 기간: 2020.11.01 ~ 2021.11.01
    - 역할
        - RFID 게이트 기반 안전보호구 운용 관리 소프트웨어 개발
        - Zigbee를 활용한 RFID 리더기 데이터 스트리밍 장치 개발
        - 출입 기록 및 근로자 DB 데이터 송수신 기능 개발
    - 주요 성과
        - 무선 통신망 구축 경험 및 DB 관련 지식 습득
    
- IoT 기술 기반 휴대용 및 이동형 컨베이어 벨트 고장진단 디바이스 개발
    - 설명: 발전소에서 발생하고 있는 작업자의 사망 사고를 줄이기 위해 안전하고
효율적인 고장 진단 시스템을 개발함
    - 주관: 한국서부발전(주)
    - 기간: 2021.08.05 ~ 2021.12.31
    - 역할
        - 휴대용 및 이동형 컨베이어 벨트 고장진단 디바이스 시스템 구상
        - 정부 R&D 과제 사업 제안서 작성
    - 주요 성과
        - 시스템 구상 경험 및 제안서 작성 요령 습득
    

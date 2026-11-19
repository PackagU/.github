# PackagU

**엘리베이터 버튼을 로봇팔로 직접 눌러 층을 이동하는 실내 자율 택배 배달 로봇**  
건국대학교 전기전자공학부 2026 종합설계 **5조**

<!-- VIDEO_SLOT: hero_gif (추후 대표 GIF로 교체) -->
<p align="center">
  <img src="assets/robot_labeled.jpg" alt="PackagU 실물 로봇 구성" width="480" />
</p>

<p align="center">
  <a href="https://github.com/PackagU/PackagU">
    <img src="https://img.shields.io/badge/Main%20Repository-PackagU%2FPackagU-1F6FEB?style=for-the-badge&logo=github&logoColor=white" alt="PackagU/PackagU 저장소 이동" />
  </a>
</p>

---

## 프로젝트 소개

**PackagU**는 건물 엘리베이터 제어 API나 승강기 패널 개조 없이, 기존 다층 건물에서 택배를 자율 배달하는 실내 이동 로봇 프로젝트다. ROS 2 Humble 기반 2륜 차동 SLAM/Nav2 주행에 4 DOF 로봇팔·웹캠 버튼 조작, 층별 자동 지도 전환, Z축 지게팔 상하차를 통합했다.

## 핵심 기능

- **다층 자율 주행 및 층별 지도 전환**: RPLiDAR A1m8 + SLAM Toolbox·Nav2 주행, 엘리베이터 이동 뒤 `/map_server/load_map` 및 AMCL 재정위로 층별 지도를 자동 교체
- **로봇팔 버튼 직접 조작**: 팔 끝 웹캠으로 호출·층 버튼과 램프를 확인하고 4 DOF 서보 로봇팔로 물리 버튼을 직접 조작
- **지게팔 택배 상하차**: Arduino Uno + TB6600 기반 Z축 지게팔(`lift_uno`)과 상승 중 초음파 높이 제한(`10 cm`)으로 팔레트·택배를 적재·하역

자세한 시스템 구조, 코드 읽기 지도, 실물·시뮬레이션 검증 결과는 [**PackagU/PackagU**](https://github.com/PackagU/PackagU)에서 확인할 수 있다.

## 팀과 역할

| 이름 | GitHub | 담당 역할 |
|---|---|---|
| **이준형** | [@JunhyungLee25](https://github.com/JunhyungLee25) | SLAM · Nav2 · 층별 자동 지도 전환 · 시뮬레이션 · 현장 시스템 통합 |
| **한수민** | [@inonewater](https://github.com/inonewater) | Fusion 360 기구 설계 · 2륜 차동 구동부 · Z축 지게팔(리프트) |
| **이성덕** | [@DuckFrog123](https://github.com/DuckFrog123) | 4 DOF 로봇팔 · 엘리베이터 버튼 인식 및 조작 |

## 기술 스택

![ROS 2 Humble](https://img.shields.io/badge/ROS2%20Humble-22314E?style=for-the-badge&logo=ros&logoColor=white)
![Nav2](https://img.shields.io/badge/Nav2-1F6FEB?style=for-the-badge&logoColor=white)
![SLAM Toolbox](https://img.shields.io/badge/SLAM%20Toolbox-2C3E50?style=for-the-badge&logoColor=white)
![Jetson Xavier NX](https://img.shields.io/badge/Jetson%20Xavier%20NX-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![OpenCR 1.0](https://img.shields.io/badge/OpenCR%201.0-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Gazebo Classic](https://img.shields.io/badge/Gazebo%20Classic-FF7300?style=for-the-badge&logoColor=white)

# PackagU

엘리베이터 버튼을 로봇팔로 직접 눌러 층을 이동하는 실내 택배 배달 로봇 프로젝트입니다.  
건국대학교 전기전자공학부 2026 종합설계 5조에서 진행했습니다.

<!-- VIDEO_SLOT: hero_gif -->
<p align="center">
  <img src="assets/robot_labeled.jpg" alt="PackagU 실물 로봇" width="460" />
</p>

<p align="center">
  <a href="https://github.com/PackagU/PackagU">
    <img src="https://img.shields.io/badge/Repository-PackagU%2FPackagU-1F6FEB?style=for-the-badge&logo=github&logoColor=white" alt="PackagU/PackagU" />
  </a>
</p>

건물 엘리베이터 API나 설비 개조 없이 다층 배달을 수행하는 것을 목표로, Jetson Xavier NX(ROS 2 Humble) 위에서 SLAM/Nav2 주행, 4 DOF 로봇팔 버튼 조작, 층별 지도 전환, Z축 지게팔 상하차를 구현했습니다.

전체 코드와 시스템 구성, 실험 결과는 [PackagU/PackagU](https://github.com/PackagU/PackagU)에 정리되어 있습니다.

### 팀원

| 이름 | GitHub | 담당 |
|---|---|---|
| 이준형 | [@JunhyungLee25](https://github.com/JunhyungLee25) | SLAM, Nav2, 층별 지도 전환, 시뮬레이션, 시스템 통합 |
| 한수민 | [@inonewater](https://github.com/inonewater) | 기구 설계(Fusion 360), 구동부, Z축 지게팔 |
| 이성덕 | [@DuckFrog123](https://github.com/DuckFrog123) | 4 DOF 로봇팔, 버튼 인식 및 조작 |

![ROS 2 Humble](https://img.shields.io/badge/ROS2%20Humble-22314E?style=for-the-badge&logo=ros&logoColor=white)
![Nav2](https://img.shields.io/badge/Nav2-1F6FEB?style=for-the-badge&logoColor=white)
![SLAM Toolbox](https://img.shields.io/badge/SLAM%20Toolbox-2C3E50?style=for-the-badge&logoColor=white)
![Jetson Xavier NX](https://img.shields.io/badge/Jetson%20Xavier%20NX-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![OpenCR 1.0](https://img.shields.io/badge/OpenCR%201.0-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Gazebo Classic](https://img.shields.io/badge/Gazebo%20Classic-FF7300?style=for-the-badge&logoColor=white)

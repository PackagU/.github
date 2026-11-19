# PackagU

엘리베이터 버튼을 4 DOF 로봇팔로 직접 눌러 층을 옮기는 실내 택배 배달 로봇이다. 건국대학교 전기전자공학부 2026 종합설계 5조가 만들었다.

<p align="center">
  <img src="assets/e2e_demo.gif" alt="PackagU 실물 배달 시연 하이라이트" height="340" />
  <img src="assets/robot_labeled.jpg" alt="PackagU 실물 로봇" height="340" />
</p>

<p align="center">
  <a href="https://github.com/PackagU/PackagU">
    <img src="https://img.shields.io/badge/Repository-PackagU%2FPackagU-1F6FEB?style=for-the-badge&logo=github&logoColor=white" alt="PackagU/PackagU" />
  </a>
</p>

건물 엘리베이터 API가 없는 환경에서 다층 배달을 수행하려고 Jetson Xavier NX(ROS 2 Humble) 위에 SLAM/Nav2 주행, 4 DOF 로봇팔 버튼 조작, 층별 지도 전환, Z축 지게팔 상하차를 얹었다. 코드와 시스템 구성, 검증 결과는 [PackagU/PackagU](https://github.com/PackagU/PackagU)에 정리했다.

### 팀원

| 이름 | GitHub | 담당 |
|---|---|---|
| 이준형 | [@JunhyungLee25](https://github.com/JunhyungLee25) | SLAM, Nav2, 층별 지도 전환, 시뮬레이션, 현장 통합 |
| 한수민 | [@inonewater](https://github.com/inonewater) | Fusion 360 기구 설계, 구동부, Z축 지게팔 |
| 이성덕 | [@DuckFrog123](https://github.com/DuckFrog123) | 4 DOF 로봇팔, 버튼 인식과 조작 |

![ROS 2 Humble](https://img.shields.io/badge/ROS2%20Humble-22314E?style=for-the-badge&logo=ros&logoColor=white)
![Nav2](https://img.shields.io/badge/Nav2-1F6FEB?style=for-the-badge&logoColor=white)
![SLAM Toolbox](https://img.shields.io/badge/SLAM%20Toolbox-2C3E50?style=for-the-badge&logoColor=white)
![Jetson Xavier NX](https://img.shields.io/badge/Jetson%20Xavier%20NX-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![OpenCR 1.0](https://img.shields.io/badge/OpenCR%201.0-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Gazebo Classic](https://img.shields.io/badge/Gazebo%20Classic-FF7300?style=for-the-badge&logoColor=white)

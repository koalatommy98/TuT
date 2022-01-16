# TuT

2022-01-07

- Jetson Nano
  - SSH 허용
  - VNC 뷰어 연결
  - RoS 설치

2022-01-16

- Slamtec의 Rplidar-A2를 이용해 패키지 설치와 동작
-  Code
  -  $ roslaunch rplidar_ros view_rplidar.launch => 실질적인 Lidar 작동을 Rvis로 보여줌.
  -  $ roslaunch rplidar_ros rplidar.launch => 라이다 작동만 시킴.
- Error
  - buffer overflow detected => https://github.com/Slamtec/rplidar_ros/issues/63 => 시리얼포트 권한 주기
  - cv_bridge Error => https://jstar0525.tistory.com/118 => open cv 경로수정

- 참고1 : https://www.jetsonhacks.com/2018/12/07/rplidar-a2-nvidia-jetson-development-kits/
- 참고2 : https://github.com/slamtec/rplidar_ros

- Hector Slam 작동
- Code
  - $ roslaunch rplidar_ros rplidar.launch => 라이다 작동
  - $ roslaunch hector_slam_launch tutorial.launch => Hector Slam 작동
  
- 참고1 : https://doongdoongeee.tistory.com/104



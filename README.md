# LIDAR
라이다 관련 정보 (ubuntu)
RPLIDAR관련 툴 설치 정보 : https://m.blog.naver.com/thumbdown/220385363246
slam 동작 : https://blog.naver.com/hwann218/222238803461
slam 동작2 : https://chat.openai.com/c/5ab0ef59-5697-4528-b301-2c483e233f5f#none
slam 동작3 (with gazebo) : https://roboticsbackend.com/ros2-nav2-generate-a-map-with-slam_toolbox/

라이다 USB포트 번호 알내기 ttyUSB* : lsusb | grep -i 'LiDAR' | wc -l
RP라이다 툴 설치 : sudo apt install ros-$ROS_DISTRO-rplidar-ros

#wsl2
WSL2에 ros2설치 : https://keep-steady.tistory.com/45?category=922869
환경 변수 임의 지정 : $env:PATH = $env:PATH + ";C:\Windows\System32"
wsl2 usb포트 연결 : https://velog.io/@pikamon/Linux-6
    중간에 에러시 : https://askubuntu.com/questions/1406205/install-usb-ip-on-ubuntu-22-04-on-windows-subsystem-for-linux


#urdf
urdf 튜토리얼 : https://navigation.ros.org/setup_guides/urdf/setup_urdf.html 
- 한국어 지원 : https://duvallee.tistory.com/10

#ROS1 Melodic
catkin_make -> source devel/setup.bash


#map server
설치 : sudo apt-get install ros-<ROS 버전>-map-server
맵 저장 : rosrun map_server map_saver -f <map_name>
맵 불러오기 (노드 설정) : rosrun map_server map_server <map_name>.yaml
-> 이후 rviz를 키고 맵 토픽 설정

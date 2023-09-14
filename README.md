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
- github : https://github.com/ros-planning/navigation2_tutorials/blob/master/sam_bot_description/launch/display.launch.py

#ROS1 Melodic                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
catkin_make -> source devel/setup.bash


#map server
설치 : sudo apt-get install ros-<ROS 버전>-map-server
맵 저장 : rosrun map_server map_saver -f <map_name>
맵 불러오기 (노드 설정) : rosrun map_server map_server <map_name>.yaml
-> 이후 rviz를 키고 맵 토픽 설정

#ubuntu server
설정 및 gui 설치 :https://shinestone.tistory.com/27
ports 오류시 : https://askubuntu.com/questions/91543/apt-get-update-fails-to-fetch-files-temporary-failure-resolving-error
ubuntu wifi: https://velog.io/@gilchris/Ubuntu-20.04-terminal%EC%97%90%EC%84%9C-wifi-%EC%9E%A1%EA%B8%B0
wifi ip 주소 알아내기 : ip a | grep inet | grep wlan

#ubuntu 원격 접속 : https://jkim83.tistory.com/131 
https://catnip-archive.tistory.com/entry/Ubuntu-Ubuntu-1804-%EB%B6%80%ED%8C%85-%EC%8B%9C-%EB%A1%9C%EA%B7%B8%EC%9D%B8-%EC%83%9D%EB%9E%B5%ED%95%98%EA%B8%B0#:~:text=%EB%A8%BC%EC%A0%80%20%EC%84%A4%EC%A0%95%EC%97%90%20%EB%93%A4%EC%96%B4%EA%B0%80%EC%84%9C%20%22Detail,%EC%84%A4%EC%A0%95%EC%9D%80%20%EB%81%9D%EC%9D%B4%20%EB%82%A9%EB%8B%88%EB%8B%A4.

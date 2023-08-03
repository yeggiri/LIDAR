# LIDAR
라이다 관련 정보 (ubuntu)
RPLIDAR관련 툴 설치 정보 : https://m.blog.naver.com/thumbdown/220385363246
slam 동작 : https://blog.naver.com/hwann218/222238803461


라이다 USB포트 번호 알내기 ttyUSB* : lsusb | grep -i 'LiDAR' | wc -l
라이다 툴 설치 : sudo apt install ros-$ROS_DISTRO-rplidar-ros

#wsl2
WSL2에 ros2설치 : https://keep-steady.tistory.com/45?category=922869
wsl2 usb포트 연결 : https://velog.io/@pikamon/Linux-6
    중간에 에러시 : https://askubuntu.com/questions/1406205/install-usb-ip-on-ubuntu-22-04-on-windows-subsystem-for-linux

# shinysdr_docker_rtlsdr
shinysdr docker for rtlsdr
dockerization steps:
1. unzip shinysdr.zip
2. build
    docker build -t shinysdr:rtlsdr .
3. run
   docker run -t -p 8100:8100 -p 8101:8101 --privileged -v /dev/bus/usb:/dev/bus/usb shinysdr:rtlsdr

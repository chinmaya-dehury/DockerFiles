# Download this docker file and build the weka_docker app with following command 
#     sudo docker build -t weka_docker .

# run the following command 
#     sudo docker run -it --rm \
#          -v /tmp/.X11-unix:/tmp/.X11-unix \
#          -e DISPLAY=unix$DISPLAY \
#	   -v $HOME/weka:/home/weka \ 	
#          --name weka \
#          weka_docker

# If any error occur related to "Gtk-WARNING **: cannot open display: :1"
# execute the following command 
#         xhost +local:docker



FROM debian:sid
RUN apt-get update && apt-get install -y \
	default-jre \
	libsvm-java \
	weka
CMD [ "weka" ]

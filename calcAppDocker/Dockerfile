# Download this docker file and build the calc_docker app with following command 
#     sudo docker build -t calc_docker .

# run the following command 
#     sudo docker run -it --rm \
#          -v /tmp/.X11-unix:/tmp/.X11-unix \
#          -e DISPLAY=unix$DISPLAY 
#          --name calc
#          calc_docker

# If any error occur related to "Gtk-WARNING **: cannot open display: :1"
# execute the following command 
#         xhost +local:docker


FROM debian:sid
RUN apt-get update && apt-get install -y gnome-calculator
CMD [ "gnome-calculator" ]

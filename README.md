sudo apt-get install libjpeg62-turbo-dev

sudo apt-get install cmake

git clone https://github.com/jacksonliam/mjpg-streamer.git 

cd ~/mjpg-streamer/mjpg-streamer-experimental

cd ~/mjpg-streamer/mjpg-streamer-experimental


sudo rm -rf /opt/mjpg-streamer

sudo mv ~/mjpg-streamer/mjpg-streamer-experimental /opt/mjpg-streamer

sudo rm -rf ~/mjpg-streamer

LD_LIBRARY_PATH=/opt/mjpg-streamer/ /opt/mjpg-streamer/mjpg_streamer -i "input_raspicam.so -fps 15 -q 50 -x 720 -y 640" -o "output_http.so -p 9000 -w /opt/mjpg-streamer/www" &


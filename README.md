# Eye-fatigue-detection
Nonintrusive methods for eye locating and tracking arithmetic in fatigue detection research
# intallation process
# step 1:
install all libarys
* scipy,opencv,numpy,imutils,pyglet,dlib
installation of Dlib libary

Pre-reqs:
* On Linux:
  * Install boost. On Ubuntu, that's sudo apt-get install libboost-all-dev
Clone the code from github:
https://github.com/NoMorningstar/Eye-fatigue-detection.git
Build the main dlib library:
cd dlib
mkdir build; cd build; cmake .. -DDLIB_USE_CUDA=0 -DUSE_AVX_INSTRUCTIONS=1; cmake --build .
Build and install the Python extensions:
cd ..
python3 setup.py install --yes USE_AVX_INSTRUCTIONS --no DLIB_USE_CUDA
At this point, you should be able to run python3 and type import dlib successfully.
## if you have python 2.7
cd ..
python setup.py install --yes USE_AVX_INSTRUCTIONS --no DLIB_USE_CUDA
# step 2
download a ring name as alarm.wav
# step 3
python eyedetection.py

This guide is for installation of geant4.10.04 in ubuntu 18.04. However, it should work for all versions of geant4.

1. Update the package lists
```bash
sudo apt-get update
```

2. Install pre-requisites
```bash
    sudo apt-get install cmake
    sudo apt-get install gcc
    sudo apt-get install g++ 
    sudo apt-get install expat
    sudo apt-get install libexpat1-dev
    sudo apt-get install default-jre
    sudo apt-get install default-jdk
    sudo apt-get install qt4-default
    sudo apt-get install cmake-qt-gui
    sudo apt-get install mesa-common-dev
    sudo apt-get install libglu1-mesa-dev
    sudo apt-get install libxmu-dev
```    

3. Download the latest geant4 source code from geant4 website
```bash
    wget "http://cern.ch/geant4-data/releases/geant4.10.04.tar.gz"
```

4. Extract the source code
```bash
tar -zxvf geant4.10.04.tar.gz
```

5.
```bash
    -DGEANT4_BUILD_MULTITHREADED=ON -DGEANT4_INSTALL_DATA=ON -DGEANT4_USE_OPENGL_X11=ON -DGEANT4_USE_QT=ON ../geant4.10.04
```

4. make -j4 
```bash
    make install                        #to install geant4
```
### Congratulations...Geant4 is now installed.

cd examples/masterbuild

cmake -DGeant4_DIR=~/geant4.9.6.p04install/lib/Geant4-9.6.4

~/geant4.9.6.p04/examples/cyliSD

make -j4

source /home/ranga/geant4.9.6.p04install/bin/geant4.sh

./cyliSD

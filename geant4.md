This guide is for installation of geant4.10.04 in ubuntu 18.04. However, it should work for all versions of geant4.

1. Update the package lists
```bash
    sudo apt-get update
```

2. Install pre-requisites
```bash
    sudo apt-get install cmake gcc g++ expat libexpat1-dev default-jre default-jdk qt4-default cmake-qt-gui mesa-common-dev libglu1-mesa-dev libxmu-dev
```    

3. Download the latest geant4 source code from geant4 website
```bash
    wget "http://cern.ch/geant4-data/releases/geant4.10.04.tar.gz"
```

4. Extract the source code
```bash
    tar -zxvf geant4.10.04.tar.gz
```

5. Make a build folder and go into that folder
```bash
    mkdir geant4build
    cd geant4build
```

6. Configure the installation
```bash
    cmake -DGEANT4_BUILD_MULTITHREADED=ON -DGEANT4_INSTALL_DATA=ON -DGEANT4_USE_OPENGL_X11=ON -DGEANT4_USE_QT=ON ../geant4.10.04
```

7. To install geant4 
```bash
    make -j4
    make install
```
4 is the number of logical processors in my CPU. Change according to your CPU.    

### Congratulations...Geant4 is now installed.

Please email me if you find any error.

---
![visitors](https://visitor-badge.glitch.me/badge?page_id=rangavirender.site.geant4)

<p align="center">
<img src="logo_v1.png" width="30">
</p>

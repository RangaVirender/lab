```bash
    #Update the package lists
    sudo apt-get update
    
    #Install pre-requisites
    sudo apt-get install dpkg-dev cmake g++ gcc binutils libx11-dev libxpm-dev libxft-dev libxext-dev libpng-dev libjpeg-dev python-dev libssl-dev libtbb-dev liblzma-dev
    
    #Download the latest root source code from cern website
    wget "https://root.cern/download/root_v6.22.00.source.tar.gz"
    
    #Extract the source code 
    tar -zxvf root_v6.22.00.source.tar.gz
    
    #Make a build folder and change to that folder
    mkdir rootbuild
    cd rootbuild
    
    #Configure the installation
    cmake ../root_v6.22.00
    
    #To install root
    make -j4 #4 is the number of cores in my CPU. Change according to your CPU
    make install
```

Congratulations…ROOT is now installed.\
Please email me if you find any error.

---

![visitors](https://visitor-badge.glitch.me/badge?page_id=rangavirender.site.tools)

<p align="center">
<img src="logo_v1.png" width="30">
</p>

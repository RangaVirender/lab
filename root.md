1. Update the package lists
```bash
    sudo apt-get update
```

2. Install pre-requisites
```bash
    sudo apt-get install dpkg-dev cmake g++ gcc binutils libx11-dev libxpm-dev libxft-dev libxext-dev libpng-dev libjpeg-dev python libssl-dev 
```

3. Download the latest root source code from cern website
```bash
    wget "https://root.cern/download/root_v6.22.00.source.tar.gz"
```

4. Extract the source code
```bash 
    tar -zxvf root_v6.22.00.source.tar.gz
```

5. Make a build folder and go into that folder
```bash 
    mkdir rootbuild
    cd rootbuild
```

6. Configure the installation
```bash
    cmake ../root_v6.22.00
```

7. To install root
```bash
    make -j4
    make install
```
4 is the number of cores in my CPU. Change according to your CPU.

Congratulations…ROOT is now installed.\
Please email me if you find any error.

---
![visitors](https://visitor-badge.glitch.me/badge?page_id=rangavirender.site.tools)

<p align="center">
<img src="logo_v1.png" width="30">
</p>

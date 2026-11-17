# 3DS-Mouse-Control
An application allowing you to control your Mac/Linux/Windows PC's mouse through your 3DS as long as both devices are on the same Wi-Fi connection.  

**Prerequisites:**  
[Python 3](https://www.python.org/downloads/)  
[Pynput](https://pypi.org/project/pynput/) `pip install pynput`  
[devkitPro](https://devkitpro.org/wiki/Getting_Started) with 3DS tools (3ds-dev)  

**Building**  
To set up, you first need to clone the repository and change the IP in `source/main.c` to your PC's local IP address.  
Then `cd` into the project directory and compile the program with `make`.  
```
cd 3DS-Mouse-Control
make
```

**Running**  
Move `3DS-Mouse-Control.3dsx` to `~/3ds/` on your SD card and run 3DS-Mouse-Control in the homebrew app.  
Then run client.py in a terminal window on your pc:  
```
cd 3DS-Mouse-Control
python3 client.py
```

Small demonstration: https://youtu.be/FoayD1Gaq6Q?si=7NgX9qDGsHmXk-E8 

**Current Development**  
I'm currently working on developing a GUI for the program on the 3DS side to allow inputting an IP address inside the application itself, removing the need to compile the program yourself to change it. 
I'm also working on a controller mode to let the 3ds work for PC games which use WASD and mouse movement.

**Future Plans**
I want to allow for using the 3DS as a proper controller in games but this will require an Apple Developer account.
I may add support for using the 3DS as a proper controller on Windows and Linux in the future.
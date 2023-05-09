---
hide:
 - toc
 - path
 - title
---


## Houdini UI Customization
- Dark Flat Theme [Site](https://axelschoterman.com/resources)<br>
- John Kunz Video [Youtube](https://www.youtube.com/watch?v=VdiEd84Kjsw)

---
## Hide Splash Screen 

Uncomment this in houdini.env
``` 
HOUDINI_NO_SPLASH = 1
```
Windows - `Documents/HoudiniXX.X/houdini.env`<br>
Linux - `home/username/HoudiniXX.X/houdini.env`

---
## Linux GPU Fix
Add this to houdini.env
```
HOUDINI_USE_HFS_OCL=0
```
---
## Houdini Linux Install
[Link](https://www.sidefx.com/faq/question/install-linux/)

> Make sure that the install file is not located in root's home folder (/root) as this will give you permission errors during the 

1. Open a Terminal.
2. Unpack the downloaded tar.gz archive.
   ```
   tar -xvf houdini-xx.x.xxx-linux_x86_64_gcc6.3.tar.gz
   ```
3. Go into the unpacked directory and run the houdini.install script using sudo.
    ```
    cd houdini-18.0.287-linux_x86_64_gcc6.3
    ```
    ```
    sudo ./houdini.install
    ```

4. To launch Houdini from the Terminal, type the following:

    ```
    cd /opt/hfsXX.X
    ```
    ```
    source houdini_setup
    ```
    ```
    houdini
    ```

---
## Delete License Keys
1. Control Panel > Administrative tools > Services.
2. Stop the following 2 services: Houdini License Client & Houdini License Server.
3. Now delete C:\Windows\keys\

---


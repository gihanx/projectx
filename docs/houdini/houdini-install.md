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

---
## Delete License Keys
1. Control Panel > Administrative tools > Services.
2. Stop the following 2 services: Houdini License Client & Houdini License Server.
3. Now delete C:\Windows\keys\

---


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
### Houde Splash

Uncomment this houdini.env | Documents/Houdini19.5/Houdini.env
``` 
HOUDINI_NO_SPLASH = 1
```
---
### Linux GPU Fix
Add this to houdini.env
```
HOUDINI_USE_HFS_OCL=0
```
---
- [Ikrima](https://ikrima.dev/)

- [Houdini Engine For Unreal](https://www.sidefx.com/docs/unreal/index.html)

- [Tokeru](https://www.tokeru.com/cgwiki/main_page)

- [John Kunz](https://wiki.johnkunz.com/index.php?title=resources)
---
### Houdini Linux Install
[Link](https://www.sidefx.com/faq/question/install-linux/)

---
### Uninstall Keys
```First off, go to Control Panel > Administrative tools > Services.
Stop the following 2 services: Houdini License Client & Houdini License Server.
Now delete the server files from the Winnt/system32/ folder. They are named
hserver.exe and sesinetd.exe
The licenses themselves are in a folder called keys, but you can leave those.
```

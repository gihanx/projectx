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
1. Control Panel > Administrative tools > Services.
2. Stop the following 2 services: Houdini License Client & Houdini License Server.
3. Now delete C:\Windows\keys\

## Steam Client

Steam CMD [**Link**](https://developer.valvesoftware.com/wiki/SteamCMD)

Steam Desktop Authenticator [**Link**](https://github.com/jessecar96/steamdesktopauthenticator)


---
## Steam Launch Arguments 
- Run it as a bat from steam dir<br>
- Disable Steam Chromium Backend 

```
start steam.exe -dev -console -nofriendsui -no-dwrite -nointro -nobigpicture -nofasthtml -nocrashmonitor -noshaders -no-shared-textures -disablehighdpi -cef-single-process -cef-in-process-gpu -single_core -cef-disable-d3d11 -cef-disable-sandbox -disable-winh264 -cef-force-32bit -no-cef-sandbox -vrdisable -cef-disable-breakpad +open steam://open/minigameslist 
```

---

## Launch Options for Steam Games

```
-NoVSync -NOSPLASH -USEALLAVAILABLECORES -malloc=system +mat_antialias 0 -NOMANSKY
```
---
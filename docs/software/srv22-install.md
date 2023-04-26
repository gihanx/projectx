---
hide:
 - toc
 - path
 - title
---

## Download the ISO
https://www.microsoft.com/en-us/evalcenter/download-windows-server-2022

---

## Remove Server Manager Startup

---

## Upgrade
```
 > DISM /online /Set-Edition:ServerStandard /ProductKey:VDYBN-27WPP-V4HQT-9VMD4-VMK7H /AcceptEula
 ```

---

## Tweaks

- C Drive index off

- Driver install

- GPEdit 
  > Disable shutdown even tracker<br>
  > Disable automatic updates<br>
  > Remove access to updates<br>
  > Remove password<br>

- Remove user password

---

## Remove Edge

```
cd %PROGRAMFILES(X86)%\Microsoft\Edge\Application\8*\Installer
```
```
setup --uninstall --force-uninstall --system-level
```

---

## Delete Features/Roles

- Defender, Sysdata Achiver
- Add .Net 3.5, DirectAPI

---

## Activate

```
slmgr.vbs -ipk VDYBN-27WPP-V4HQT-9VMD4-VMK7H
```
```
slmgr.vbs -skms kms.srv.crsoo.com
```
```
slmgr.vbs -ato
```

---
---
hide:
 - toc
 - path
 - title
---

Download the ISO
https://www.microsoft.com/en-us/evalcenter/download-windows-server-2022

Remove Server Manager Startup

Upgrade
```
 > DISM /online /Set-Edition:ServerStandard /ProductKey:VDYBN-27WPP-V4HQT-9VMD4-VMK7H /AcceptEula
 ```

c drive index off

driver install

gpedit [disable shutdown even tracker, disable automatic updates, remove access to updates, remove password]

control panel [remove user password]

remove edge
```
> cd %PROGRAMFILES(X86)%\Microsoft\Edge\Application\8*\Installer
> setup --uninstall --force-uninstall --system-level
```

server manager [remove defender and etc]
server manager add .net 3.5 / directapi

Activate
```
> slmgr.vbs -ipk VDYBN-27WPP-V4HQT-9VMD4-VMK7H
> slmgr.vbs -skms kms.srv.crsoo.com
> slmgr.vbs -ato
```
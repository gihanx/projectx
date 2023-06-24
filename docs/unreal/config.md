---
hide:
 - toc
 - path
 - title
---
## Set Default Project to DX11 instead of DX12

- Navigate to ```..\UE_5.2\Engine\Config```

- Past the Following text in the ``BaseEngine.ini``
```
[/Script/WindowsTargetPlatform.WindowsTargetSettings]
DefaultGraphicsRHI=DefaultGraphicsRHI_DX11
```

> - This file defines the default settings for core and engine-level features
> - These settings are overridden by a project's DefaultEngine.ini file and per-platform overrides
> - Some of these settings can be modified from the project settings in the editor
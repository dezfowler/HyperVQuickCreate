# Additional Hyper-V QuickCreate options.

This code is NOT endorsed nor supported by Microsoft or Canonical. I think it's safe and use it on my own systems. However, your mileage may vary and should only USE THIS CODE AT YOUR OWN RISK (and make sure you have a good backup!).

PRs and feedback are welcomed.

# Getting started

The most important step here is to install the `GalleryLocations.reg` file. This file will create or overwrite the `GalleryLocatoins` registry value stored at `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Virtualization`. Because it's a multi-string value, the data is encoded and hard to read. The values being installed are:

```
https://go.microsoft.com/fwlink/?linkid=851584
https://raw.githubusercontent.com/natethegreat44/HyperVQuickCreate/refs/heads/main/UbuntuGalleryHyperV.json
```

The first one is the default used by Hyper-V QuickCreate and the second one contains the new Ubuntu options that are housed in this repo. You can use a local file path here, too, such as `C:\Users\me\MyCustomGallery.json`.

# References

https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/user-guide/custom-gallery#build-a-new-gallery-source

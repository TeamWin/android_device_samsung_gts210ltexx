## TWRP device tree for Samsung Galaxy Tab S2 9.7 2015 (LTE)
## gts210ltexx

Add to `.repo/local_manifests/gts210ltexx.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="TeamWin/android_device_samsung_gts210ltexx" path="device/samsung/gts210ltexx" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_gts210ltexx-eng
mka recoveryimage
```

Kernel source: https://github.com/LineageOS/android_kernel_samsung_gts2/tree/cm-14.1

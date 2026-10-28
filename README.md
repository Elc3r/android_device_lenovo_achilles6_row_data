# Lenovo TB-X606X — LineageOS 19.1 device tree

Unofficial Lenovo Tab M10 FHD Plus (2nd Gen), **TB-X606X LTE**,
product `achilles6_row_data`. Based on
`lenovo-mt6765/android_device_lenovo_achilles6_row_data`, commit
`162ed79f078d29880d84491bc7f82f4e765f0f23`.

Use the matching common tree, proprietary inputs and `lenovo-tb-x606x`
integration repo for pinned manifests, platform patches, instructions and
tested status. This tree on an unmodified LineageOS checkout is insufficient.

```bash
source build/envsetup.sh
lunch lineage_achilles6_row_data-userdebug
m -j4 bacon
```

The selected kernel and Wi-Fi module come from the official Lenovo Software Fix
firmware `TB_X606X_S301085_230919_BMP.zip` (September 2023). The other seven
modules match that package byte-for-byte. DTB/DTBO remain inherited prebuilts.
Kernel SHA256: `c9b07e553475373f27946b4c6e4cc03d634558cefc6d0900132a46ae1cd8d8dd`.
The matching TWRP manifest imports this same kernel. Android boot, Wi-Fi
association, Enforcing and required HAL registration passed the new-build audit;
this is not a complete hardware regression test.
This repository does not
provide complete corresponding kernel source or a kernel-source build.
No security update is implied. Do not reuse the images for X606F/X606FA.

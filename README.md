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

Kernel, DTB/DTBO and modules are inherited prebuilts. This repository does not
provide complete corresponding kernel source or a kernel-source build.
No security update is implied. Do not reuse the images for X606F/X606FA.

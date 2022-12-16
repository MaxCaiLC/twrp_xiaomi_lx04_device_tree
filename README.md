XiaoMi XiaoAiTongXue LX04
===============
```
By : MaxCaiLC & FatdeadPanda
```
The LX04 (codename _"lx04"_) is a Smart speaker from XiaoMi.

![Picture](https://file-fatdeadpanda.netlify.app/mi_lx04.jpg)

This is a Minimal Device Tree for building TWRP for XiaoMi XiaoAiTongXue LX04 (Codename: mi_lx04). I used TWRP by multirom and TWRP for Asus Zenpad 3S 10 from rakomancha to finally build a working tree for XiaoMi XiaoAiTongXue LX04.

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A35 | Quad-Core | MT8167
Memory       | 1GB RAM
Shipped Android Version | 8.1
Storage      | 4GB
Display      | 4.0

This branch is for building TWRP.

### Thanks to:
 * FatdeadPanda
 * Myself

### To build: 

```
$ mkdir twrp

$ cd twrp

$ repo init -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-8.1

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-8.1

After that sync your sources:

$ repo sync

Download or clone this repository, go to /twrp/device and create xiaomi/mi_lx04. Copy this repo to your created folder

Build your recovery:

$ source build/envsetup.sh

& lunch omni_lx04-eng

make clean && make recoveryimage
```

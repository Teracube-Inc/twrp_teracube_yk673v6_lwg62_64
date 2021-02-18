# TWRP device tree for Teracube 2e (yk673v6\_lwg62\_64)

<p align="center">
  <img height="600" src="/preview.png?raw=true">
</p>

Basic        | Spec Sheet
------------:|:-------------------------
CPU          | Octa-core processor @ 1.8Ghz
Chipset      | MediaTek Helio A25
GPU          | PowerVR Rogue GE8320
Memory/RAM   | 4 GB
Storage      | 64 GB
Battery      | 4000 mAh (Removable)
Dimensions   | 155.2mm x 73.3mm x 10.1mm
Display      | 6.1” HD+ IPS Display (720X1560)
Rear Camera  | 13+8 MP
Front Camera | 8 MP
Release Date | November 2020


## Build instructions
- Initialize the source tree -
  ```bash
  repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0
  ```
  You may optionally pass `--depth=1` to save space, like so:
  ```bash
  repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0
  ```
- Clone this repository -
  ```bash
  git clone https://github.com/Teracube-Inc/twrp_teracube_yk673v6_lwg62_64 device/teracube/yk673v6_lwg62_64
  ```
- Build -
  ```bash
  source build/envsetup.sh
  export ALLOW_MISSING_DEPENDENCIES=true
  lunch omni_yk673v6_lwg62_64-eng
  mka recoveryimage
  ```
- Flash -
  Follow the instructions on [Teracube forums](https://community.myteracube.com/t/advanced-users-only-twrp-recovery-root-for-teracube-2e/1729)


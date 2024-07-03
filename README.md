# Assumptions

SkylineOS for Harley Davidson is provided and contracted by a separate vendor.

They use QNX which is a RealTime OS similar to Linux owned by BlackBerry.

# Mounting Images

Image Files in Package:
```
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/recovery_mifs_hyp_la.img
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/recovery_ifs2_la.img
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/visteon-recovery-la.img
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/recovery_system_la.img

vendor.img: Android sparse image, version: 1.0, Total of 262144 4096-byte output blocks in 23 input chunks.
```

## QNX6 Image Files

```
visteon-recovery-la.img: DOS/MBR boot sector
recovery_system_la.img: DOS/MBR boot sector
recovery_ifs2_la.img: data
recovery_mifs_hyp_la.img: ELF 64-bit LSB executable, ARM aarch64, version 1 (SYSV), statically linked, no section header
```

### Create Virtual Python Environment

```
$ python3 -m venv venv
$ source ./venv/bin/activate
```

### Install QNXMount

```
$ pip install qnxmount
$ sudo apt install fuse
```

### Create Temporary Mount Point

```
$ mkdir temp-mount
```

### Mount Image File

```
$ python  -m qnxmount qnx6 vidteon-recovery-la.img ./temp-mount
```

explore!

## Android Image Files

### Install Andorid SDK Utilities

```
$ apt install android-sdk-libsparse-utils
```

## Convert Sparse File.
```
$ simg2img vendor.img new_vendor.img
```
##  Create Mount Point
```
$ mkdir temp-mount2
```
## Mount via loop device
```
$ mount -o loop new_vendor.img temp-mount2
```

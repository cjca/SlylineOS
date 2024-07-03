# Assumptions

SkylineOS for Harley Davidson is provided and contracted by a separate vendor.

They use QNX which is a RealTime OS similar to Linux owned by BlackBerry.


# Locations

Files are in for the most part host/flash/sw_part2, (INSTANA_240002213D)

for VR___NA_240200552D, files are in sw_part13.
for CAL__NA_240402088D, files are in sw_part0.

CAL  is 'Calibration'.  Most files are csv files.

# Mounting Images

Image Files in Package:
```
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/recovery_mifs_hyp_la.img
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/recovery_ifs2_la.img
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/visteon-recovery-la.img
./INSTANA_240002213D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/recovery_system_la.img


./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part1/reflash_rec_pkg/recovery_ifs2_la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part1/reflash_rec_pkg/recovery_system_la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part1/reflash_rec_pkg/visteon-recovery-la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part1/reflash_rec_pkg/recovery_mifs_hyp_la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/ifs2_la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/mifs_hyp_la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/system.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/boot_la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/vendor.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/vbmeta.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/visteon-platform-la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/system_la.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/persist_qnx.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/boot.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/persist.img
./INSTANA_240002237D/orch-pkg/update-pkg/devices/host/flash/sw_part2/reflash_pkg/userdata.img


```

## QNX6 Image Files

```
visteon-recovery-la.img: DOS/MBR boot sector
recovery_system_la.img: DOS/MBR boot sector
recovery_ifs2_la.img: data
recovery_mifs_hyp_la.img: ELF 64-bit LSB executable, ARM aarch64, version 1 (SYSV), statically linked, no section header


abl.elf:                 ELF 32-bit LSB executable, ARM, version 1 (SYSV), statically linked, no section header
abl_fastboot.elf:        ELF 32-bit LSB executable, ARM, version 1 (SYSV), statically linked, no section header
aop.mbn:                 ELF 32-bit LSB executable, ARM, EABI5 version 1 (GNU/Linux), statically linked, no section header
boot.img:                Android bootimg, kernel (0x8000), ramdisk (0x1000000), page size: 4096, cmdline (console=hvc0,115200 debug user_debug=31 loglevel=9 print-fatal-signals=1 androidboot.console=ttyAMA0 androidboot.hardware=qcom )
boot_la.img:             Android bootimg, kernel, page size: 2048
BTFM.bin:                DOS/MBR boot sector, code offset 0x3c+2, OEM-ID "MSDOS5.0", Bytes/sector 4096, sectors/cluster 4, root entries 512, Media descriptor 0xf8, sectors/FAT 3, sectors/track 63, heads 255, sectors 16384 (volumes > 32 MB), serial number 0xbc614e, unlabeled, FAT (16 bit)
cmnlib64.mbn:            ELF 64-bit LSB shared object, ARM aarch64, version 1 (SYSV), static-pie linked, no section header
cmnlib.mbn:              ELF 32-bit LSB shared object, ARM, EABI5 version 1 (SYSV), static-pie linked, no section header
devcfg_auto.mbn:         ELF 64-bit LSB executable, ARM aarch64, version 1 (SYSV), statically linked, no section header
dspso.bin:               Linux rev 1.0 ext4 filesystem data, UUID=af32c008-2a39-7e5b-a5dc-201456d93103, volume name "dsp" (extents) (large files)
ifs2_la.img:             data
km4virt.mbn:             ELF 64-bit LSB shared object, ARM aarch64, version 1 (SYSV), dynamically linked, no section header
logfs_ufs_8mb.bin:       DOS/MBR boot sector, code offset 0x3c+2, OEM-ID "MSDOS5.0", Bytes/sector 4096, root entries 512, sectors 1280 (volumes <=32 MB), Media descriptor 0xf8, sectors/FAT 1, sectors/track 1, heads 1, hidden sectors 16, serial number 0xd27355ea, unlabeled, FAT (12 bit)
manifest.xml:            exported SGML document, ASCII text
manifest.xml.tmpl:       exported SGML document, ASCII text
mifs_hyp_la.img:         ELF 64-bit LSB executable, ARM aarch64, version 1 (SYSV), statically linked, no section header
multi_image.mbn:         ELF 32-bit LSB no file type, ARM, version 1 (SYSV)
NON-HLOS.bin:            DOS/MBR boot sector, code offset 0x3c+2, OEM-ID "MSDOS5.0", Bytes/sector 4096, sectors/cluster 4, root entries 512, Media descriptor 0xf8, sectors/FAT 6, sectors/track 63, heads 255, sectors 43520 (volumes > 32 MB), serial number 0xbc614e, unlabeled, FAT (16 bit)
persist.img:             Linux rev 1.0 ext4 filesystem data, UUID=0562acb0-eca1-436b-8ed4-2f652300d28e (extents) (large files) (huge files)
persist_qnx.img:         DOS/MBR boot sector
qupv3fw.elf:             ELF 32-bit LSB executable, QUALCOMM DSP6, version 1 (SYSV), statically linked, no section header
storsec.mbn:             ELF 32-bit LSB shared object, ARM, EABI5 version 1 (SYSV), dynamically linked, no section header
system.img:              Android sparse image, version: 1.0, Total of 655360 4096-byte output blocks in 60 input chunks.
system_la.img:           DOS/MBR boot sector
tz.mbn:                  ELF 64-bit LSB executable, ARM aarch64, version 1 (GNU/Linux), statically linked, no section header
uefi_sec.mbn:            ELF 32-bit LSB shared object, ARM, EABI5 version 1 (SYSV), dynamically linked, no section header
updatemanifest.sh:       POSIX shell script, ASCII text executable
userdata.img:            Android sparse image, version: 1.0, Total of 1310720 4096-byte output blocks in 24 input chunks.
vbmeta.img:              data
vendor.img:              Android sparse image, version: 1.0, Total of 262144 4096-byte output blocks in 23 input chunks.
visteon-platform-la.img: DOS/MBR boot sector




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
$ sudo apt install android-sdk-libsparse-utils
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

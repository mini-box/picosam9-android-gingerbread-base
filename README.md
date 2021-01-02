# Android 2.3.x for Atmel AT91 based devices

 Android changes to run under Atmel AT91 including usb WIFI and Ethernet. This MCU is also powering 
 Mini-Box.com *picoPC*. See: http://arm.mini-box.com
 
# Related repositories
  A special Bootstrap is needed to boot from sdcard and a special modified kernel which implements [sam9g45](https://www.arm.linux.org.uk/developer/machines/list.php?id=3838) machine architecture.
  
  
  - Bootstrap: https://github.com/mini-box/picosam9-bootstrap
  - Kernel: https://github.com/mini-box/picosam9-kernel
  - Toolchain: https://github.com/mini-box/picosam9-toolchain
  
# Building
 For system prerequisites see https://source.android.com/setup/build/older-versions.
 
    . build/envsetup.sh
    make update-api (only on first compilation)
    TARGET_PRODUCT=picopc m


# Original source
This Android source is derived from AOSP with extensive changes. To obtain original source:

    repo init -u git://android.git.kernel.org/platform/manifest.git -b android-2.3.3_r1
    repo sync





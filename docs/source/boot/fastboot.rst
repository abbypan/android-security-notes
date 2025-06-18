fastboot
============

开发者选项里的 oem unlock开关，标识是否允许进行设备解锁(allow)

fastboot oem unlock / fastboot flashing unlock 执行设备解锁，变更设备是否已bootloader解锁的状态(status)

doc
-------

- `Flash with Fastboot <https://source.android.com/docs/setup/test/running>`_
- `Lock and unlock the bootloader <https://source.android.com/docs/core/architecture/bootloader/locking_unlocking#locking-bootloader>`_
- `Android Fastboot Mode Commands with Examples <https://meghtechnologies.com/blog/fastboot-mode-commands-with-examples/>`_
- `avb.c: trusty_write_lock_state <https://cs.android.com/android/platform/superproject/main/+/main:external/trusty/bootloader/ql-tipc/avb.c?q=trusty_write_lock_state`_
- `rockchip android avb <https://github.com/ericsonj/tools/blob/master/linux/Linux_SecurityAVB/readme.md>`_
- `How To Unlock Bootloader Via Fastboot Method On Android <https://www.getdroidtips.com/unlock-bootloader-via-fastboot-on-android/>`_
- `fastboot.cpp <https://cs.android.com/android/platform/superproject/main/+/main:system/core/fastboot/fastboot.cpp?q=fastboot%20oem%20unlock>`_


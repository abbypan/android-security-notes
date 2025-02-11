AVB unlock
===========

信任链: prk -> pik -> {psk, puk}

psk 负责vbmeta镜像签名，puk 负责解锁。

psk certificate 中包含 product_id。

permanent_attribute 中包含 version, prk, product_id。secure boot时，permanent_attribute必须由efuse/otp校验。

puk certificate 中包含 product id、且usage标记为unlock。

unlock credential 由 puk 对 unlock_challenge 签名。注意unlock_challenge的结构体以及device_id关联。


参考资料
-------------

- `avb_manager.h <https://android.googlesource.com/trusty/app/avb/+/refs/heads/main/avb_manager.h>`_
- `avb_atx_types <https://android.googlesource.com/platform/external/avb/+/nougat-iot-release/libavb_atx/avb_atx_types.h>`_
- `avb_cert_validate.c <https://android.googlesource.com/platform/external/avb/+/refs/heads/main/libavb_cert/avb_cert_validate.c>`_
- `rk AVB Reference <https://github.com/ericsonj/tools/blob/master/linux/Linux_SecurityAVB/readme.md>`_
- `at_auth_unlock.py <https://android.googlesource.com/platform/external/avb/+/refs/heads/main/tools/at_auth_unlock.py>`_
- `avb_atx_generate_test_data <https://cs.android.com/android/platform/superproject/+/android14-qpr3-release:external/avb/test/avb_atx_generate_test_data?q=%20permanent_attributes.bin>`_
- `avb_cert_types <https://android.googlesource.com/platform/external/avb/+/refs/heads/main/libavb_cert/avb_cert_types.h>`_
- `avb test <https://android.googlesource.com/platform/external/avb/+/refs/heads/main/test>`_




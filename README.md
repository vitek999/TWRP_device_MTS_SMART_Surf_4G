TWRP device tree for SMART_Surf_4G (c) hyperion70 - 2017

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | 1.0GHz Quad-Core MT6735P
GPU     | Mali-T720
Memory  | 1GB RAM
Shipped Android Version | 5.1
Storage | 8GB
Battery | 1800 mAh
Display | 5.0" 1280 x 720 px
Camera  | 5MPx + 2MPx, LED Flash

=================================

Для сборки recovery TWRP 3.1.x.x в исходниках СМ заменить bootable/recovery на соответствующую из omirom.
To recovery  build in the Lineage OS sources, you need a busybox-7.1 (https://github.com/omnirom/android_external_busybox/tree/android-7.1)

	$ cd $(LOCAL_DIR)/device/MTS/SMART_Surf_4G
	$ . apply-patch.sh

	$ export WITH_SU=true
    $ breakfast SMART_Surf_4G
	$ make clean
	$ make recoveryimage 

Thanks @fichl for twrp theme pack

TWRP device tree for SMART_Surf_4G (c) hyperion70 - 2017

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | 1.0GHz Quad-Core MT6735P
GPU     | Mali-T720
Memory  | 1GB RAM
Shipped Android Version | 5.1
Storage | 8GB
Battery | 1900 mAh
Display | 5.0" 1280 x 720 px
Camera  | 5MPx + 2MPx, LED Flash

=================================

To recovery build in the Lineage OS 14.1 sources

	$ cd $(SOURCE)/bootable
    $ rm -rf recovery
    $ git clone https://github.com/omnirom/android_bootable_recovery recovery
    $ cd recovery
    $ git apply -v ../../device/MTS/SMART_Surf_4G/01-twrp_recovery_mtk.patch
    $ cd ../..

	$ . build/envsetup.sh
    $ breakfast SMART_Surf_4G
	$ make clean
	$ make recoveryimage

## Thanks to:
 * @blastagator
 * @DeckerSU
 * @olegsvs
 * @ariafan
 * @DeepFlex
 * @Zormax


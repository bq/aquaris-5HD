WHAT IS THIS?
=============

Linux Kernel source code for the device bq Aquaris 5HD

BUILD INSTRUCTIONS?
===================

Specific sources are separated by branches and each version is tagged with it's corresponding number. First, you should
clone the project:

	$ git clone git@github.com:bq/aquaris-5HD.git

After it, choose the version you would like to build:

	$ cd aquaris-5HD/
	$ git checkout 1.0.3_20140116-1954
	
Finally, build the kernel:
	
	$ cd kernel/
	$ rm -rf out/
	$ mkdir out/
	$ TARGET_PRODUCT=lcsh89_we_jb2 MTK_ROOT_CUSTOM=../mediatek/custom make O=out

WHAT IS THIS?
=============

Linux Kernel source code for the device bq Aquaris 5HD

BUILD INSTRUCTIONS?
===================

Specific sources are separated by branches and each version is tagged with it's corresponding number. First, you should
clone the project:

        $ git clone git@github.com:bq/aquaris-5HD.git

##After it, choose the version you would like to build:

### Version 1.x (Jelly Bean)


        $ cd aquaris-5HD/
        $ git checkout 1.0.3_20140116-1954

Build the kernel:

        $ cd kernel/
        $ rm -rf out/
        $ mkdir out/
        $ TARGET_PRODUCT=lcsh89_we_jb2 MTK_ROOT_CUSTOM=../mediatek/custom make O=out


### Version 2.x (KitKat)


        $ cd aquaris-5HD/
        $ git checkout 2.0.0_20140911-1054

Build the kernel:

        $ ./makeMtk -t lcsh89_wet_kk n k

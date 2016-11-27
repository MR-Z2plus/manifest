
Getting Started
---------------

To get started with TWRP & MULTI-ROM, you'll need to get
familiar with [Git and Repo](http://source.android.com/download/using-repo).

To initialize your local repository using the MULTI-ROM trees, use a command like this:

    mkdir MR-Z2Plus

    cd MR-Z2Plus

    repo init -u git://github.com/MR-Z2plus/manifest.git -b mr

Then to sync up:

    repo sync -c -f -j8 --force-sync --no-clone-bundle

For build MultiROM:
     
     . build/envsetup.sh
     
     lunch tipsy_z2_plus-userdebug

The following is from: https://github.com/Tasssadar/multirom/wiki/Porting-MultiROM

make recoveryimage # builds the recovery image

make multirom trampoline # builds multirom binary and build trampoline - MultiROM's init daemon

make multirom_zip # builds multirom and trampoline and installation ZIP file

make multirom_uninstaller # builds uninstaller ZIP

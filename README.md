# Li Mee's Modified Pixel Experience #

Focusing on fixing some localization problems in mainland China, as well as some details, also may add some fuctions that I think are useful.

> Thanks for the Pixel Experience project.

### Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/LiMeeROMDev/manifest -b twelve

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash
# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```

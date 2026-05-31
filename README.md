# OctaviOS Android Manifest #

### Initialize OctaviOS ###

**Initialize full repository (useful for developers)**
```
repo init -u https://github.com/OctaviOS-Plus/android_manifest -b 16 --git-lfs
```

**If you want to save space, use this instead**
```
repo init -u https://github.com/OctaviOS-Plus/android_manifest -b 16 --git-lfs --depth 1
```

### Sync Sauce ###
```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch
```

### Build ROM ###
```
. build/envsetup.sh

brunch device
```

## Now Build and Enjoy! ##

# ClovaOS Android Manifest #

### Initialize ClovaOS ###

**Initialize full repository (useful for developers)**
```
repo init -u https://github.com/ClovaOS/android_manifest -b 17.0 --git-lfs
```

**If you want to save space, use this instead**
```
repo init -u https://github.com/ClovaOS/android_manifest -b 17.0 --git-lfs --depth 1
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

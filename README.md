# OctaviOS Android Manifest #

![Banner](https://github.com/user-attachments/assets/c77bfc71-86e7-4e2d-b80b-cbeb9d4e32b1)

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

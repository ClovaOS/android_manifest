# ClovaOS Android Manifest

### Initialize ClovaOS

**Full repository checkout (recommended for developers)**

```bash
repo init -u https://github.com/ClovaOS/android_manifest -b 17.0
```

**Shallow checkout (saves disk space)**

```bash
repo init -u https://github.com/ClovaOS/android_manifest -b 17.0 --depth=1
```

> A shallow checkout downloads limited Git history. Use the full checkout if you plan to develop, merge upstream changes, or work with Git history.

### Sync Sauce

```bash
repo sync -c -j$(nproc --all) --no-clone-bundle --no-tags --optimized-fetch
```

### Build ROM

**Set up the build environment:**

```bash
source build/envsetup.sh
```

**Select your device and preferred build variant:**

```bash
lunch clova_<device>-cp2a-<variant>
```

Replace `<device>` with your device codename and `<variant>` with one of the following:

- `user` – Production build
- `userdebug` – Development build with debugging capabilities
- `eng` – Engineering build with additional debugging features

**Example for Sony Xperia 1 V (pdx234):**

```bash
lunch clova_pdx234-cp2a-userdebug
```

**Build ClovaOS:**

```bash
m bacon
```

## Now Build and Enjoy!

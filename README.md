# MoonOS #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/MoonOS-Project/manifest -b 11

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch moon_$device-userdebug

# Build the code
$ mka bacon -jX
```


# Xiaomi Mi 8 Lite manifest
* Android version: 10
* Branch: lineage-17.1 (LineageOS 17.1)

### Sync ###

```bash
# Initialize LineageOS 17.1
repo init -u git://github.com/LineageOS/android.git -b lineage-17.1

# Initialize Mi 8 Lite repository
rm -rf .repo/local_manifests
git clone https://github.com/mi8lite/manifest .repo/local_manifests -b lineage-17.1

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

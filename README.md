
## How to build:
```shell
source build/envsetup.sh
lunch lineage_etab5-userdebug
mka bacon
```

## How to fix build errors:
- `Assertion 'cnt < (sizeof (_nl_value_type_LC_TIME) / sizeof (_nl_value_type_LC_TIME[0]))' failed.`
  - Run "`export LC_ALL=C`" before building

- dex2oat errors
  - Downgrade your Linux kernel to some version like 5.10 (I was using Debian 12 with 6.1.0 kernel, you can install kernel 5.10 using bullseye's apt repositories)

## Good luck! :3

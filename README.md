# rtl8822bu-edimax

rtl8822bu wifi/bt driver from edimax

This driver is from Edimax website:

https://www.edimax.com/edimax/merchandise/merchandise_detail/data/edimax/global/wireless_adapters_ac1200_dual-band/ew-7822ulc/

# Changes

1. add `CONFIG_PLATFORM_ARM_RPI3` for general arm64 configuration.
2. add `EXTRA_CFLAGS += -Wno-bool-operation` to suppress warning.

# Usage

```
make CROSS_COMPILE=aarch64-linux-gnu- KSRC=<path/to/kernel/source>
```


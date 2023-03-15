# trojan-go-for-openwrt

## 编译

从 OpenWrt 的 [SDK](https://openwrt.org/docs/guide-developer/obtain.firmware.sdk) 编译
```bash
cd openwrt-sdk

# 获取源码
git clone https://github.com/Typhonling/trojan-go-for-openwrt.git package/trojan-go-for-openwrt

# 选中 Network -> chinadns-ng
make menuconfig

# 编译 chinadns-ng
make package/trojan-go-for-openwrt/{clean,compile} V=s

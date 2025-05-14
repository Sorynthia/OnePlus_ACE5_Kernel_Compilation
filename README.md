# OnePlus ACE5 内核编译项目 🚀

[![编译状态](https://github.com/Sorynthia/OnePlus_ACE5_Kernel_Compilation/actions/workflows/Build-SukiSU.yml/badge.svg)](https://github.com/Sorynthia/OnePlus_ACE5_Kernel_Compilation/actions/workflows/Build-SukiSU.yml)

这是一个针对一加ACE5手机的自动化内核编译项目，使用GitHub Actions每日构建集成SukiSU-Ultra的内核。

## ✨ 特性

- 🔄 **每日自动编译**：北京时间次日0点自动构建最新内核
- 🛡️ **SukiSU-Ultra**：基于SukiSU-Ultra分支的KernelSU集成
- 📁 **SUSFS支持**：提供更强大的文件系统挂载功能
- 🔧 **VFS补丁**：优化虚拟文件系统性能
- 📱 **全功能KPM**：内核级进程管理支持
- ⚡ **优化性能**：针对一加ACE5优化的内核配置

## 📋 构建信息

- **平台**：Qualcomm SM8650 (Pineapple)
- **Android版本**：Android 14
- **内核版本**：Linux 6.1
- **定制名称**：Sorynthia

## 💿 如何使用

### 刷入方式

1. **使用Recovery/TWRP刷入**：
   - 下载`AnyKernel3_KernelSU_*.zip`文件
   - 进入Recovery模式
   - 选择刷入zip包并选择下载的zip文件
   - 重启设备

2. **使用Fastboot刷入**：
   - 下载`Image_KernelSU_*.zip`文件并解压
   - 连接手机并进入Fastboot模式
   - 执行命令：`fastboot flash init_boot 解压后的init_boot_Image.img文件路径`
   - 重启设备

### 管理应用

推荐使用[SukiSU-Ultra管理器](https://github.com/ShirkNeko/SukiSU-Ultra/releases)来管理root权限。

## ⚠️ 注意事项

- 如果构建的内核版本没变，不必更新
- 仅保留最近3个版本的构建
- 首次安装后请重启设备以完成KernelSU初始化
- 如遇问题，可尝试清除KernelSU应用数据后重启

## 🔄 自动化流程

此项目使用GitHub Actions自动化工作流程：
- 每天自动编译最新内核
- 自动发布到GitHub Releases
- 自动清理旧版本，保留最新的7个版本

## 🙏 致谢

- [KernelSU团队](https://github.com/tiann/KernelSU)
- [SukiSU-Ultra项目](https://github.com/ShirkNeko/SukiSU-Ultra)
- [AnyKernel3](https://github.com/osm0sis/AnyKernel3)
- 一加开源社区

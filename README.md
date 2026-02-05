# STM32 定时器外部时钟 (TIM External Clock)

## 项目描述

基于 STM32 的定时器外部时钟配置项目，演示如何配置和使用 STM32 的定时器外部时钟源功能。

## 开发环境

- **IDE**: Keil MDK-ARM
- **MCU**: STM32 系列（STM32F10x）
- **编程语言**: C
- **标准库**: STM32 标准外设库

## 项目结构

```
TIM-/
├── User/           # 用户代码（主程序）
│   ├── main.c                  # 主程序入口
│   ├── stm32f10x_conf.h        # STM32 配置文件
│   ├── stm32f10x_it.c          # 中断服务程序
│   └── stm32f10x_it.h          # 中断服务程序头文件
├── Hardware/       # 硬件驱动代码
│   ├── Key.c/Key.h             # 按键驱动
│   ├── LED.c/LED.h             # LED 驱动
│   └── OLED.c/OLED.h           # OLED 显示驱动
├── Library/        # STM32 标准外设库
├── Start/          # 启动文件
├── System/         # 系统配置文件
├── Project.uvprojx # Keil 项目文件
└── README.md       # 项目说明文档
```

## 如何使用

### 1. 打开项目

使用 Keil MDK-ARM 打开项目文件：
```
Project.uvprojx
```

### 2. 编译项目

在 Keil MDK-ARM 中：
- 点击菜单栏 `Project` -> `Build Target`
- 或按快捷键 `F7` 进行编译

### 3. 下载到开发板

- 连接 STM32 开发板到电脑
- 在 Keil 中点击 `Flash` -> `Download`
- 或按快捷键 `F8` 下载程序到目标板

### 4. 运行调试

- 点击 `Debug` -> `Start/Stop Debug Session`
- 或按快捷键 `Ctrl+F5` 开始调试

## 功能特性

- ⏱️ 定时器外部时钟配置
- 🔌 硬件外设驱动支持（LED、按键、OLED）
- 📊 实时显示功能
- 🔧 完整的项目工程配置

## 注意事项

1. 确保已安装 Keil MDK-ARM 开发环境
2. 需要安装对应的 STM32 器件支持包
3. 根据实际硬件连接调整 GPIO 引脚配置
4. 确保开发板供电正常

## 许可证

本项目仅供学习和参考使用。

## 贡献

欢迎提交 Issue 和 Pull Request 来改进项目。

---

**开发日期**: 2024  
**作者**: STM32 开发团队

# Arduino UI 系统示例

基于Arduino的交互式UI系统，使用Axeuh_UI库实现多级菜单、动画效果和3D渲染功能。

## 功能特性
- 🖥️ OLED显示支持（128x64）
- 🎮 支持矩阵键盘/摇杆输入
- 📜 多级菜单系统（含子菜单嵌套）
- 🎨 GIF动画显示支持
- 🎛️ 参数滑动条调节
- 🧊 实时3D立方体渲染
- 📖 多行文本显示窗口
- ⌨️ 中文拼音输入键盘
- 🔋 状态栏显示（可扩展）

## 硬件要求
- Arduino开发板（ESP32系列已验证）
- SSD1306 OLED屏幕（SPI/I2C）
- 矩阵键盘或摇杆模块
- 按键开关（用于确认操作）

## 依赖库
- [Axeuh_UI](https://github.com/作者仓库地址)（需自行安装）
- U8g2图形库（Arduino Library Manager安装）
- Wire（内置库）

## 快速开始

### 硬件连接
```cpp
/* OLED引脚配置（SPI示例） */
#define CS_PIN   5
#define DC_PIN   17
#define RES_PIN  16

/* 输入控制引脚 */
#define BTN_PIN     25  // 确认键
#define JOY_Y_PIN   35  // 上下方向
#define JOY_X_PIN   34  // 左右方向

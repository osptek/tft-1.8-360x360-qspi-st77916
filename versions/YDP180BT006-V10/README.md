<p align="left"><img alt="OSPTEK" src="./images/logo.png" width="200" /></p>

<h1 align="center">OSPTEK 1.8″ TFT 360×360（ST77916 · QSPI）</h1>

<p align="center"><b>圆形 TFT 模组 · QSPI · ST77916</b></p>

<p align="center"><a href="./README_EN.md">English</a> | 简体中文 · <a href="../../README.md">规格族索引</a></p>

<p align="center">
  <img alt="Size: 1.8 inch" src="https://img.shields.io/badge/Size-1.8%22-3498DB?style=flat-square" />
  <img alt="Resolution: 360x360" src="https://img.shields.io/badge/Resolution-360%C3%97360-8E44AD?style=flat-square" />
  <img alt="Interface: QSPI" src="https://img.shields.io/badge/Interface-QSPI-27AE60?style=flat-square" />
  <img alt="Driver: ST77916" src="https://img.shields.io/badge/Driver-ST77916-E7352C?style=flat-square" />
</p>

<p align="center"><img alt="OSPTEK 1.8 寸 360×360 TFT QSPI 模组（ST77916）宣传图" src="./images/product.png" width="640" /></p>

## 目录

- [产品简介](#产品简介)
- [规格参数](#规格参数)
- [示例工程](#示例工程)
- [仓库结构](#仓库结构)
- [相关资料](#相关资料)
- [购买链接](#购买链接)
- [技术支持](#技术支持)

---

## 产品简介

OSPTEK **1.8 寸 360×360 TFT** 是一款 **QSPI** 接口彩色显示模组，显示驱动为 **ST77916**，触摸驱动为 **CST816D**。方形分辨率适合圆形穿戴表盘与紧凑 HMI 等场景。

规格标识（仓库名）：`tft-1.8-360x360-qspi-st77916`

当前模组版本：**YDP180BT006-V10**。电气与接口细节以 [`docs/YDP_180_BT_006_V10_a22cc8dde1.pdf`](./docs/YDP_180_BT_006_V10_a22cc8dde1.pdf) 为准。盖板外形（YDP180BT008A-V10 / YDP180BT008B-V10）见下方相关资料，不单独开分支。

## 规格参数

| 项目 | 规格 |
| ---- | ---- |
| 尺寸 | 1.8 英寸 |
| 类型 | TFT（彩色透射） |
| 分辨率 | 360×360 |
| 接口 | QSPI |
| 驱动 IC | ST77916 |
| 触摸驱动 | CST816D |

> 完整外形尺寸、FPC 定义、供电与时序以产品规格书 / 驱动手册为准。

## 示例工程

| 说明 | 路径 |
| ---- | ---- |
| ESP32-S3 · ST77916 QSPI + LVGL8 | [`examples/esp32s3-idf5_st77916-qspi_lvgl8/`](./examples/esp32s3-idf5_st77916-qspi_lvgl8/) |
| ESP32-S3 · ST77916 QSPI + esp-lvgl-adapter / LVGL8 | [`examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8/`](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8/) |
| ESP32-S3 · ST77916 QSPI + esp-lvgl-adapter / LVGL9 | [`examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9/`](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9/) |
| ESP32-S3 · LVGL8 + TE 防撕裂 | [`examples/with-te/esp32s3-idf5_st77916-qspi_lvgl8_lcd-with-te/`](./examples/with-te/esp32s3-idf5_st77916-qspi_lvgl8_lcd-with-te/) |
| ESP32-S3 · esp-lvgl-adapter LVGL8 + TE | [`examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8_lcd-with-te/`](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8_lcd-with-te/) |
| ESP32-S3 · esp-lvgl-adapter LVGL9 + TE | [`examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9_lcd-with-te/`](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9_lcd-with-te/) |

## 仓库结构

```text
tft-1.8-360x360-qspi-st77916/                                # 仓库根（导航见 ../../README.md）
└── versions/
    └── YDP180BT006-V10/                                # 本料号完整资料
        ├── README.md
        ├── README_EN.md
        ├── images/
        ├── docs/
        └── examples/
```

## 相关资料

### 本产品资料

| 资料 | 链接 |
| ---- | ---- |
| 产品规格书（YDP180BT006-V10） | [`docs/YDP_180_BT_006_V10_a22cc8dde1.pdf`](./docs/YDP_180_BT_006_V10_a22cc8dde1.pdf) |
| 外形图（YDP180BT008A-V10 · 2.5D 盖板） | [`docs/YDP180BT008A-V10.pdf`](./docs/YDP180BT008A-V10.pdf) |
| 外形图（YDP180BT008B-V10 · 圆盖板） | [`docs/YDP180BT008B-V10.pdf`](./docs/YDP180BT008B-V10.pdf) |
| 驱动 IC 数据手册（ST77916） | [`docs/ST77916_SPEC_V1.0.pdf`](./docs/ST77916_SPEC_V1.0.pdf) |
| 触摸 IC 数据手册（CST816D） | [`docs/CST_816_D_V1_0_2_1b06dfb078.pdf`](./docs/CST_816_D_V1_0_2_1b06dfb078.pdf) |
| 初始化序列（文本） | [`docs/ST77916_BOE_1.8_360x360_QSPI_init_V1.6.txt`](./docs/ST77916_BOE_1.8_360x360_QSPI_init_V1.6.txt) |

### 示例工程

- [ESP32-S3 ST77916 QSPI + LVGL8](./examples/esp32s3-idf5_st77916-qspi_lvgl8/)
- [ESP32-S3 ST77916 QSPI + esp-lvgl-adapter / LVGL8](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8/)
- [ESP32-S3 ST77916 QSPI + esp-lvgl-adapter / LVGL9](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9/)
- [ESP32-S3 LVGL8 + TE](./examples/with-te/esp32s3-idf5_st77916-qspi_lvgl8_lcd-with-te/)
- [ESP32-S3 esp-lvgl-adapter LVGL8 + TE](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8_lcd-with-te/)
- [ESP32-S3 esp-lvgl-adapter LVGL9 + TE](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9_lcd-with-te/)

## 购买链接

<p align="center">
  <a href="https://shop110742373.taobao.com/"><img alt="淘宝官方店铺" src="https://img.shields.io/badge/淘宝-官方店铺-FF6A00?style=for-the-badge" /></a>
  &nbsp;&nbsp;
  <a href="https://www.aliexpress.com/store/1105701619"><img alt="速卖通官方店铺" src="https://img.shields.io/badge/速卖通-官方店铺-FF6A00?style=for-the-badge" /></a>
</p>

**国内（淘宝）**

- 店铺：[鱼鹰光电工厂店](https://shop110742373.taobao.com/)

**海外（AliExpress）**

- 店铺：[OSPTEK Official Store](https://www.aliexpress.com/store/1105701619)

## 技术支持

- 技术支持 / 产品咨询：<luyu@osptek.com>
- QQ 技术交流群：**985881096**
- 公司官网：<https://osptek.com/>
- 有任何问题，都可以在本仓库 Issues 中提问

---

<p align="center"><sub>© 2026 OSPTEK 鱼鹰光电 · 本仓库资料采用 CC BY 4.0 许可</sub></p>

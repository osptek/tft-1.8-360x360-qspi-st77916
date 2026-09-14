<p align="left"><img alt="OSPTEK" src="./images/logo.png" width="200" /></p>

<h1 align="center">OSPTEK 1.8″ TFT 360×360 (ST77916 · QSPI)</h1>

<p align="center"><b>Round TFT module · QSPI · ST77916</b></p>

<p align="center"><a href="./README.md">简体中文</a> | English · <a href="../../README_EN.md">Family index</a></p>

<p align="center">
  <img alt="Size: 1.8 inch" src="https://img.shields.io/badge/Size-1.8%22-3498DB?style=flat-square" />
  <img alt="Resolution: 360x360" src="https://img.shields.io/badge/Resolution-360%C3%97360-8E44AD?style=flat-square" />
  <img alt="Interface: QSPI" src="https://img.shields.io/badge/Interface-QSPI-27AE60?style=flat-square" />
  <img alt="Driver: ST77916" src="https://img.shields.io/badge/Driver-ST77916-E7352C?style=flat-square" />
</p>

<p align="center"><img alt="OSPTEK 1.8″ 360×360 TFT QSPI module (ST77916) product image" src="./images/product.png" width="640" /></p>

## Contents

- [Overview](#overview)
- [Specifications](#specifications)
- [Sample projects](#sample-projects)
- [Repository layout](#repository-layout)
- [Resources](#resources)
- [Buy](#buy)
- [Support](#support)

---

## Overview

OSPTEK **1.8″ 360×360 TFT** is a **QSPI** color display module driven by **ST77916**, with touch controller **CST816D**. The square resolution suits round wearables and compact HMI.

Spec ID (repository name): `tft-1.8-360x360-qspi-st77916`

Current module version: **YDP180BT006-V10**. Electrical and interface details follow [`docs/YDP_180_BT_006_V10_a22cc8dde1.pdf`](./docs/YDP_180_BT_006_V10_a22cc8dde1.pdf). Cover-glass outlines (YDP180BT008A-V10 / YDP180BT008B-V10) are listed under Resources and do not get their own branches.md`](./MODULE_VERSION.md)). Electrical and interface details follow [`docs/YDP_180_BT_006_V10_a22cc8dde1.pdf`](./docs/YDP_180_BT_006_V10_a22cc8dde1.pdf).

## Specifications

| Item | Spec |
| ---- | ---- |
| Size | 1.8 inch |
| Type | TFT (color, transmissive) |
| Resolution | 360×360 |
| Interface | QSPI |
| Driver IC | ST77916 |
| Touch IC | CST816D |

> Full outline, FPC definition, power, and timing follow the product datasheet / driver IC datasheet.

## Sample projects

| Description | Path |
| ---- | ---- |
| ESP32-S3 · ST77916 QSPI + LVGL8 | [`examples/esp32s3-idf5_st77916-qspi_lvgl8/`](./examples/esp32s3-idf5_st77916-qspi_lvgl8/) |
| ESP32-S3 · ST77916 QSPI + esp-lvgl-adapter / LVGL8 | [`examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8/`](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8/) |
| ESP32-S3 · ST77916 QSPI + esp-lvgl-adapter / LVGL9 | [`examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9/`](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9/) |
| ESP32-S3 · LVGL8 + TE | [`examples/with-te/esp32s3-idf5_st77916-qspi_lvgl8_lcd-with-te/`](./examples/with-te/esp32s3-idf5_st77916-qspi_lvgl8_lcd-with-te/) |
| ESP32-S3 · esp-lvgl-adapter LVGL8 + TE | [`examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8_lcd-with-te/`](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8_lcd-with-te/) |
| ESP32-S3 · esp-lvgl-adapter LVGL9 + TE | [`examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9_lcd-with-te/`](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9_lcd-with-te/) |

## Repository layout

```text
tft-1.8-360x360-qspi-st77916/                                # repo root (nav: ../../README_EN.md)
└── versions/
    └── YDP180BT006-V10/                                # full materials for this part number
        ├── README.md
        ├── README_EN.md
        ├── images/
        ├── docs/
        └── examples/
```

## Resources

### Product files

| Resource | Link |
| ---- | ---- |
| Product datasheet (YDP180BT006-V10) | [`docs/YDP_180_BT_006_V10_a22cc8dde1.pdf`](./docs/YDP_180_BT_006_V10_a22cc8dde1.pdf) |
| Outline drawing (YDP180BT008A-V10 · 2.5D cover) | [`docs/YDP180BT008A-V10.pdf`](./docs/YDP180BT008A-V10.pdf) |
| Outline drawing (YDP180BT008B-V10 · round cover) | [`docs/YDP180BT008B-V10.pdf`](./docs/YDP180BT008B-V10.pdf) |
| Driver IC datasheet (ST77916) | [`docs/ST77916_SPEC_V1.0.pdf`](./docs/ST77916_SPEC_V1.0.pdf) |
| Touch IC datasheet (CST816D) | [`docs/CST_816_D_V1_0_2_1b06dfb078.pdf`](./docs/CST_816_D_V1_0_2_1b06dfb078.pdf) |
| Init sequence (text) | [`docs/ST77916_BOE_1.8_360x360_QSPI_init_V1.6.txt`](./docs/ST77916_BOE_1.8_360x360_QSPI_init_V1.6.txt) |

### Samples

- [ESP32-S3 ST77916 QSPI + LVGL8](./examples/esp32s3-idf5_st77916-qspi_lvgl8/)
- [ESP32-S3 ST77916 QSPI + esp-lvgl-adapter / LVGL8](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8/)
- [ESP32-S3 ST77916 QSPI + esp-lvgl-adapter / LVGL9](./examples/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9/)
- [ESP32-S3 LVGL8 + TE](./examples/with-te/esp32s3-idf5_st77916-qspi_lvgl8_lcd-with-te/)
- [ESP32-S3 esp-lvgl-adapter LVGL8 + TE](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl8_lcd-with-te/)
- [ESP32-S3 esp-lvgl-adapter LVGL9 + TE](./examples/with-te/esp32s3-idf5_st77916-qspi_esp-lvgl-adapter_lvgl9_lcd-with-te/)

## Buy

<p align="center">
  <a href="https://www.aliexpress.com/store/1105701619"><img alt="AliExpress store" src="https://img.shields.io/badge/AliExpress-Official_Store-FF6A00?style=for-the-badge" /></a>
  &nbsp;&nbsp;
  <a href="https://shop110742373.taobao.com/"><img alt="Taobao store" src="https://img.shields.io/badge/Taobao-Official_Store-FF6A00?style=for-the-badge" /></a>
</p>

**Overseas (AliExpress)**

- Store: [OSPTEK Official Store](https://www.aliexpress.com/store/1105701619)

**China (Taobao)**

- Store: [鱼鹰光电工厂店](https://shop110742373.taobao.com/)

## Support

- Technical support / product inquiry: <luyu@osptek.com>
- QQ group (China): **985881096**
- Website: <https://osptek.com/>
- Feel free to open an Issue in this repository if you have any questions

---

<p align="center"><sub>© 2026 OSPTEK · Materials in this repository are licensed under CC BY 4.0</sub></p>

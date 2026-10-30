# Changelog
All notable changes to this project will be documented in this file.

## [Unreleased]

- 启用 `lavfi` 输入设备与 `sine` / `anullsrc` 音源滤镜（改 `--disable-avdevice` → `--enable-avdevice`，并 `--enable-indev=lavfi`、`--enable-filter=sine/anullsrc`）。精简版 ffmpeg 现支持 `ffmpeg -f lavfi -i sine=…/anullsrc=…` 生成测试音频，修复下游 musicSAK 测试套件在定制构建下因 `lavfi` 缺失而整批失败的问题。仍保持仅音频、静态、~4-5MB 的精简定位。


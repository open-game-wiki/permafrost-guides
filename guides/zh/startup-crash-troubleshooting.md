---
title: "Permafrost 启动崩溃：DX11、DX12 与 DLSS 检查"
description: "按官方补丁核对 Permafrost 启动崩溃，尝试有出处的 DX11 临时方式，并区分显卡问题、系统拦截与不受支持的平台。"
category: "Technical"
badge: "资料核验 · 2026-10-28"
readingTime: "约 4 分钟"
publishDate: "2026-10-28"
updatedDate: "2026-10-28"
lang: "zh"
---


## 先分清失败发生在哪里
记录游戏版本、系统、显卡与驱动、启动参数及准确报错。启动崩溃、长时间游玩变慢、Windows 安全拦截需要不同证据。本页基于 2026-10-28 核对的开发者说明，未经本站硬件复现。

## DLSS Multi Frame Generation 启动崩溃
“Crash, Quest and Voiceover Fixes” 公告宣布修复开启 **DLSS Multi Frame Generation** 时的启动崩溃。先安装可用补丁，再复试相同场景；若仍失败，报告版本与设置。该说明不代表所有 DirectX 或显卡崩溃都已修复。

## 官方 DX11 临时方式
开发者 **Known Issues**（10 月 16 日更新）建议启动崩溃时尝试 `-dx11`：
1. 在 Steam 库右击 Permafrost，打开属性。
2. 在通用中先记下现有启动选项。
3. 尝试 `-dx11`，不要同时保留冲突的 DirectX 开关，再复试启动。
4. 记录结果；需要对照时只移除自己新增的选项，保留原有配置。

这是历史开发者临时办法，不承诺提速，也不能由此推断受支持的渲染特性或固定帧率提升。

## 能进入 Video 设置时
同一置顶帖建议尝试 Multi-Frame-Generation-Type、Super Resolution、降低画质和调整 V-Sync。记下原始值，每次只改一个，才能看出哪项影响崩溃。显卡驱动更新从对应厂商核对。

## Linux、Proton 和 Steam Deck
置顶帖说明 Linux 不获官方支持。DX11 参数不能证明 Proton 兼容，也不构成 Steam Deck 已验证预设。规格与测量记录建议见[配置和 Deck 说明](/zh/guides/system-requirements-steam-deck/)。

## 明确安全报错或仍无改善
Windows 弹出安全提示时，保留原文并使用官方支持渠道；不要把普通黑屏判断为安全拦截，也不要将关闭系统防护作为常规步骤。

按开发者要求，通过[支持上传入口](https://filehub.toplitz-productions.com/)提供版本、报错、调整过的参数、显卡驱动及是否在菜单前发生，分享前检查日志。不要为测试渲染而删除存档或覆盖云冲突。

## 来源
[最新官方补丁](https://steamcommunity.com/app/2254990/announcements/) · [10 月 16 日更新的 Known Issues](https://steamcommunity.com/app/2254990/discussions/0/588440207635776246/)。进入游戏后卡进度可查[任务状态表](/zh/guides/quest-bugs-and-fixes/)。

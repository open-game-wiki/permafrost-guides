---
title: "Startup Crashes: DX11, DX12 & DLSS Checks"
description: "Check Permafrost startup crashes against official patch notes, try the documented DX11 workaround, and separate graphics failures from unsupported setups."
category: "Technical"
badge: "SOURCE CHECK · 2026-10-28"
readingTime: "4 min read"
publishDate: "2026-10-28"
updatedDate: "2026-10-28"
lang: "en"
---


## First identify the failure
Record your game build, operating system, GPU/driver, launch options and exact error. A startup crash, a long-session slowdown and a Windows security block need different evidence. This guide is based on developer notes checked October 28, 2026, not a reproduced hardware test.

## DLSS Multi Frame Generation startup crash
“Crash, Quest and Voiceover Fixes” announces a fix for startup crashes when **DLSS Multi Frame Generation** is enabled. First install the available patch and retry the same case. If it still fails, report your build and settings; the release note does not establish a fix for every DirectX or GPU crash.

## Official DX11 workaround
The developer's **Known Issues**, updated October 16, recommends `-dx11` for startup crashes:
1. In Steam Library, right-click Permafrost and open Properties.
2. Under General, record any existing Launch Options before changing them.
3. Try `-dx11` without combining conflicting DirectX switches, then retry the same launch.
4. Note the result. Remove only the option you added if you want to compare again; retain your original options.

This is a historical developer workaround, not a promised performance upgrade. Do not infer unsupported rendering features or a fixed FPS gain.

## If the game reaches its Video settings
The same pinned post suggests testing graphics options such as Multi-Frame-Generation-Type and Super Resolution, lower quality and V-Sync changes. Record the starting settings and change one at a time so the report identifies what affected the crash. Check available GPU-driver updates through the GPU vendor.

## Linux, Proton and Steam Deck
The pinned post says Linux is not officially supported. A DX11 launch option does not prove Proton compatibility or a verified Steam Deck preset. For hardware specifications and a useful measurement checklist, see [requirements and Deck notes](/guides/system-requirements-steam-deck/).

## Explicit security error or no improvement?
If Windows shows a security warning, preserve the exact message and use the official support channel. Do not treat a generic black screen as proof of a security block or disable system protections as a routine crash step.

Send the build, error, changed options, GPU/driver and whether it occurs before the menu through the developer's [support upload](https://filehub.toplitz-productions.com/) when requested. Review logs before sharing. Do not delete saves or overwrite a Cloud conflict to test rendering.

## Sources
[Latest official patches](https://steamcommunity.com/app/2254990/announcements/) · [Known Issues, updated October 16](https://steamcommunity.com/app/2254990/discussions/0/588440207635776246/). For progress blocks after launching, use the [quest-status guide](/guides/quest-bugs-and-fixes/).

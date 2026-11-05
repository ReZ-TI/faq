---
id: FAQ-COM-013
locale: zh-CN
status: draft
audience: public_candidate
owner: kelvinchen1119
evidence_checked_on: 2026-11-05
reviewed_by: null
reviewed_at: null
sources:
  - ../sources/README.md
---

# FAQ-COM-013 · Matter over Thread 的设备需要网关吗？

> 待审核草稿，尚未发布到官网。

## 答案

支持 Matter over Thread 的设备可以直接加入 Apple Home 等支持 Thread 的生态，不需要厂商网关，也不需要依赖云端。如果现场同时有 Tuya Zigbee 版本，建议配一台 Home Assistant 主机加 Zigbee 网关，把两类设备统一到一个界面控制。是否需要另外加 Thread 边界路由，取决于现场已有的 Thread 设备和网络覆盖，把点位图或户型发给我们可以一起确认。

## 适用范围

支持 Matter over Thread 的型号。不能由此推断全部产品都免网关。

## 依据与待确认（内部核验，不随答案对外发布）

- 依据：[来源与已确认业务规则](../sources/README.md)。
- 待确认：定时功能在设备端还是 App 端按型号不同；边界路由型号是否随单提供，需与产品线确认。

[对应英文](../en/FAQ-COM-013.md) · [返回目录](README.md)

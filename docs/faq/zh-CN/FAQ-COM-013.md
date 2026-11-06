---
id: FAQ-COM-013
locale: zh-CN
status: draft
audience: public_candidate
owner: kelvinchen1119
evidence_checked_on: 2026-11-06
reviewed_by: null
reviewed_at: null
sources:
  - https://www.home-assistant.io/integrations/thread/
  - https://www.home-assistant.io/integrations/zha/
  - ../sources/README.md
  - https://support.apple.com/en-ie/102078
  - https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj
---

# FAQ-COM-013 · Matter over Thread 的设备需要网关吗？

> 待审核草稿，尚未发布到官网。

## 答案

取决于现场是否已有兼容的边界路由，不能只看我们的设备。Matter over Thread 设备要接入某个生态，需要有该生态支持的 Thread 边界路由：现场已有兼容的 Apple 家居中枢或兼容边界路由时可以复用，不需要我们另配厂商网关；如果现场只有 Thread 灯泡、手机本身又不支持 Thread，就接不进去。Apple 场景还要注意机型：只有部分支持 Thread 的 Apple 设备能做本地配对与控制，自动化与远程访问仍然需要家居中枢（如 HomePod、Apple TV 或兼容的边界路由）。把现场已有的中枢/边界路由型号、手机型号和控制平台告诉我们，我们可以一起确认是否需要补设备。

接入涂鸦时，选用支持 Matter over Thread 和相应设备类型的兼容涂鸦网关。

若同时使用 Tuya Zigbee 设备，建议另配 Home Assistant 主机加我们的 Thread Dongle 统一控制。Thread Dongle 用于 Matter over Thread 的接入；Zigbee 设备通过与 Home Assistant 兼容的 Zigbee 网关或协调器接入，业务同事会根据您已有的设备确认具体配套。两种协议与涂鸦接入的区别见 [FAQ-COM-012](FAQ-COM-012.md)。

## 适用范围

支持 Matter over Thread 的型号；能否免厂商网关取决于现场生态、手机型号与已有边界路由，不能由此推断全部产品在任意环境都免网关。

## 依据与待确认（口径说明，不随答案对外发布）

- 问题来源：近期客户询价中重复出现的问题。
- 业务确认：负责人 kelvinchen1119 于 2026-11-06 确认兼容涂鸦网关接入路径，以及同时使用 Tuya Zigbee 时推荐 Home Assistant 主机配合我司 Thread Dongle 的方案，见[来源说明](../sources/README.md)。
- 产品资料核对：我司 Thread Dongle 用于将 Matter over Thread 设备接入 Home Assistant；具体 Zigbee 接入通道按现场设备配套。
- 公开技术依据：[Home Assistant Thread 接入](https://www.home-assistant.io/integrations/thread/)与 [ZHA / Zigbee 协调器](https://www.home-assistant.io/integrations/zha/)。
- 公开技术依据：[涂鸦 Matter 互通说明](https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj)；Zigbee 接入及 Home Assistant 方案按现场设备评估。
- 外部依据：Apple 关于从便携设备添加配件的说明 <https://support.apple.com/en-ie/102078>（Thread 机型要求、本地配对与中枢/远程访问的区别）。
- 待业务确认：各型号定时在设备端还是 App 端；随单是否提供边界路由。

[对应英文](../en/FAQ-COM-013.md) · [返回目录](README.md)

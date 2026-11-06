---
id: FAQ-COM-012
locale: zh-CN
status: draft
audience: public_candidate
owner: kelvinchen1119
evidence_checked_on: 2026-11-06
reviewed_by: null
reviewed_at: null
sources:
  - ../sources/README.md
  - https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj
  - https://developer.tuya.com/en/docs/iot/Matter_technical_framework?id=Kd5alv7fmhgl9
---

# FAQ-COM-012 · 你们的 Matter 产品能接入涂鸦吗？

> 待审核草稿，尚未发布到官网。

## 答案

通常可以。涂鸦已支持 Matter，我们的 Matter over Thread 产品通常可通过支持 Matter over Thread 的兼容涂鸦网关接入涂鸦生态。接入前需核对网关型号、固件、App 版本、手机系统，以及对相应第三方 Matter 设备类型和所需功能的支持情况。

通过 Matter 接入涂鸦，与设备本身同时支持 Tuya Zigbee 和 Matter over Thread 是两回事。目前我们的标准供货版本不支持在同一设备上同时使用这两种协议；如有同机双协议需求，需要单独提出定制开发需求，按具体型号评估。请提供产品型号、涂鸦网关型号及希望实现的功能，我们协助确认方案。

## 适用范围

适用于提供 Matter 控制版本的产品。私人定制灯具须先确认实际选择了 Matter 版本。涂鸦接入能力以网关、App、手机系统和设备类型的实际支持为准；具体型号的认证覆盖分别核对。

## 依据与待确认（口径说明，不随答案对外发布）

- 业务确认：负责人 kelvinchen1119 于 2026-11-06 确认 Matter 产品通常可通过兼容涂鸦网关接入；标准版本不同时支持 Tuya Zigbee 与 Matter over Thread，同机双协议须单独定制评估。见[来源说明](../sources/README.md)。
- 公开技术依据：[涂鸦 Matter 产品互通说明](https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj)及 [Matter 架构与平台支持表](https://developer.tuya.com/en/docs/iot/Matter_technical_framework?id=Kd5alv7fmhgl9)。网关及 App/手机系统的支持范围需要核对。
- 待逐单确认：目标网关、具体设备类型与功能、认证覆盖，以及双协议定制的可行性、费用、起订量和交期。

[对应英文](../en/FAQ-COM-012.md) · [返回目录](README.md)

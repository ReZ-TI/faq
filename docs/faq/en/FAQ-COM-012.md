---
id: FAQ-COM-012
locale: en
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

# FAQ-COM-012 · Can your Matter products connect to Tuya?

> Draft pending review. Not published to the website.

## Answer

Usually, yes. Tuya supports Matter, and our Matter over Thread products can generally join the Tuya ecosystem through a compatible Tuya gateway with Matter over Thread support. Before pairing, confirm the gateway model and firmware, app version, phone operating system, and support for the relevant third-party Matter device type and required functions.

Connecting to Tuya through Matter is different from running Tuya Zigbee and Matter over Thread simultaneously on the same device. Our standard product versions do not currently support both protocols at the same time. If you need this, it requires a separate custom-development request and an assessment for the specific model. Please share the product model, Tuya gateway model and intended functions so we can confirm a suitable solution.

## Scope

Products offered with a Matter control option. For custom lighting, first confirm that the selected configuration is the Matter version. Tuya connectivity depends on the gateway, app, phone operating system and supported device type. Certification coverage must be checked for each model.

## Business confirmation and open items (not published with the answer)

- Business confirmation: on 2026-11-06, kelvinchen1119 confirmed general Tuya connectivity through a compatible gateway and that standard versions do not run Tuya Zigbee and Matter over Thread simultaneously; dual-protocol requirements need a separate custom-development assessment. See [Sources](../sources/README.md).
- Public technical references: [Tuya Matter interoperability](https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj) and [Matter architecture and platform support](https://developer.tuya.com/en/docs/iot/Matter_technical_framework?id=Kd5alv7fmhgl9). Check the gateway, app and phone-platform support for the project.
- Confirm per order: gateway, device type and functions, certification coverage, and the feasibility, cost, MOQ and lead time of dual-protocol custom development.

[Chinese version](../zh-CN/FAQ-COM-012.md) · [Index](README.md)

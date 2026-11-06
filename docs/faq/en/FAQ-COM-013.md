---
id: FAQ-COM-013
locale: en
status: draft
audience: public_candidate
owner: kelvinchen1119
evidence_checked_on: 2026-11-06
reviewed_by: null
reviewed_at: null
sources:
  - ../sources/README.md
  - https://support.apple.com/en-ie/102078
  - https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj
---

# FAQ-COM-013 · Do Matter over Thread devices need a gateway?

> Draft pending review. Not published to the website.

## Answer

It depends on whether the site already has a compatible Thread border router — it is not only about our device. A Matter over Thread device needs a Thread border router supported by the ecosystem it joins: if the site already has a compatible Apple home hub or a compatible border router, that can be reused and no vendor gateway from us is needed; if the site only has Thread bulbs and the phone itself does not support Thread, the device cannot be joined. On Apple platforms the model also matters: only certain Thread-capable Apple devices can pair and control locally, while automation and remote access still require a home hub such as a HomePod, an Apple TV or a compatible border router. Tell us the hub or border router already on site, the phone model and the control platform, and we can confirm whether anything needs to be added. 

For Tuya, use a compatible Tuya gateway that supports Matter over Thread and the relevant device types. If the site also contains Tuya Zigbee devices, check the gateway's Zigbee support as well. A Home Assistant solution can also be evaluated for unified control. See [FAQ-COM-012](FAQ-COM-012.md).

## Scope

Models supporting Matter over Thread. Whether a vendor gateway can be skipped depends on the ecosystem on site, the phone model and the existing border router; this does not imply that all products work without a gateway in any environment.

## Business confirmation and open items (not published with the answer)

- Where the question comes from: a question repeated in recent customer enquiries.
- Business confirmation: kelvinchen1119 confirmed the Matter over Thread route through a compatible Tuya gateway on 2026-11-06. See [Sources](../sources/README.md).
- Public technical reference: [Tuya Matter interoperability](https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj). Zigbee connectivity and any Home Assistant solution are assessed for the site.
- External reference: Apple support article on adding accessories from a mobile device <https://support.apple.com/en-ie/102078> (Thread-capable model requirements, local pairing versus hub-dependent automation and remote access).
- Pending business confirmation: whether schedules run on-device or in the app; whether a border router is included with an order.

[Chinese version](../zh-CN/FAQ-COM-013.md) · [Index](README.md)

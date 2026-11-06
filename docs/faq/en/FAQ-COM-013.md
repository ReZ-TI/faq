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
  - https://www.home-assistant.io/integrations/thread/
  - https://www.home-assistant.io/integrations/zha/
  - ../sources/README.md
  - https://support.apple.com/en-ie/102078
  - https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj
---

# FAQ-COM-013 · Do Matter over Thread devices need a gateway?

> Draft pending review. Not published to the website.

## Answer

It depends on whether the site already has a compatible Thread border router — it is not only about our device. A Matter over Thread device needs a Thread border router supported by the ecosystem it joins: if the site already has a compatible Apple home hub or a compatible border router, that can be reused and no vendor gateway from us is needed; if the site only has Thread bulbs and the phone itself does not support Thread, the device cannot be joined. On Apple platforms the model also matters: only certain Thread-capable Apple devices can pair and control locally, while automation and remote access still require a home hub such as a HomePod, an Apple TV or a compatible border router. Tell us the hub or border router already on site, the phone model and the control platform, and we can confirm whether anything needs to be added.

For Tuya, use a compatible Tuya gateway that supports Matter over Thread and the relevant device types.

If you also use Tuya Zigbee devices, we recommend adding a Home Assistant host together with our Thread Dongle for unified control. The Thread Dongle provides the Matter over Thread connection; Zigbee devices connect through a Zigbee gateway or coordinator compatible with Home Assistant. Our sales team will confirm the required setup based on your existing devices. See [FAQ-COM-012](FAQ-COM-012.md) for the distinction between the protocols and Tuya connectivity.

## Scope

Models supporting Matter over Thread. Whether a vendor gateway can be skipped depends on the ecosystem on site, the phone model and the existing border router; this does not imply that all products work without a gateway in any environment.

## Business confirmation and open items (not published with the answer)

- Where the question comes from: a question repeated in recent customer enquiries.
- Business confirmation: on 2026-11-06, kelvinchen1119 confirmed compatible Tuya-gateway connectivity and the recommendation to use a Home Assistant host with our Thread Dongle when Tuya Zigbee devices are also present. See [Sources](../sources/README.md).
- Product information checked: our Thread Dongle connects Matter over Thread devices to Home Assistant. The Zigbee connection is configured for the equipment on site.
- Public technical references: [Home Assistant Thread](https://www.home-assistant.io/integrations/thread/) and [ZHA / Zigbee coordinators](https://www.home-assistant.io/integrations/zha/).
- Public technical reference: [Tuya Matter interoperability](https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj). Zigbee connectivity and any Home Assistant solution are assessed for the site.
- External reference: Apple support article on adding accessories from a mobile device <https://support.apple.com/en-ie/102078> (Thread-capable model requirements, local pairing versus hub-dependent automation and remote access).
- Pending business confirmation: whether schedules run on-device or in the app; whether a border router is included with an order.

[Chinese version](../zh-CN/FAQ-COM-013.md) · [Index](README.md)
